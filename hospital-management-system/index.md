# Hospital Management System

Hospital Management System (HMS) is a python based project built on Django framework. It is a web based system that facilitates managing the functioning of the hospital. This system integrates all the information regarding patients, doctors and admin staffs into one framework.

The users of a hospital management system is divided into three categories:

* Hospital Administration
* Doctors
* Patient

## Hospital Administrator

Admin user can sign-up their account. With this credentials, they can login to the application. No Approval is required for this account. The account is auto activated on sign-up.

Admin user have the following privileges on Doctor users:

Admin can: 

	* Register a doctor user
	* Can view the doctor profile
	* Also approve a doctor account to login
	* At the same time they can reject the doctor account, if not want to approve it
	* Finally admin can delete a doctor account

In addition to above access, Admin have the following privileges on Patient users.

Admin can:

	* Admit a patient
	* View patient profile
	* Approve a patient to sign-in
	* Also reject a patient, if not want to approve it.
	* Similar to admit a patient, Admin can also discharge a patient who was admitted.

Apart from above permissions for admin, he can generate invoice and can download the generated invoice. Generating invoice can be based on medical cost, room charge, doctor charge and other charges. In addition to this, admin can book, view and approve an appointment for a patient.


## Doctor

Doctor user can apply for a job in hospital by sign-up in the web app. But for login into the app, his application has to be approved by an admin user. Then only a doctor can login.

Doctor can:

	* Only view their patient details (symptoms, name, mobile ) assigned to them by admin.
	* Can view their discharged(by admin) patient list.
	* Also they can view their Appointments, booked by admin.

Apart from viewing patient and appointments, Doctor can delete their Appointment, when they attended their appointment.


## Patient

Patient user can access the web app by sign-up similar to Doctor. But they can login only when an admin approves his account.

Patient can:

	* View assigned doctor's details like such as specialization, mobile and his address.
	* Also he can view his booked appointment status to know whether his appointent is pending or confirmed by admin.

Moreover, patient can view and download his invoice bill as PDF. But for this, the patient has to be discharged by admin. In addition to the above, patient can book his appointments. But to get it confirmed, approval has to be done by admin.

