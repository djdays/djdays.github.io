# Hospital Management System

Hospital Management System (HMS) is a python based project built on Django framework. It is a web based system that facilitates managing the functioning of the hospital. This system integrates all the information regarding patients, doctors and admin staffs into one framework.

The users of a hospital management system is divided into three categories:

* Hospital Administration
* Doctors 
* Patients

## Hospital Administrator

Admin user can sign-up their account. With this credentials, they can login to the application. No Approval is required for this account. The account is auto activated on sign-up.

Admin user have the following privileges on Doctor users:

Admin can 

	* Register a doctor user
	* Can view the doctor profile
	* Also approve a doctor account to login
	* At the same time they can reject the doctor account, if not want to approve it
	* Finally admin can delete a doctor account

Similary, Admin have the following privileges on Patient users.

Admin can

	* Admit a patient
	* View patient profile
	* Approve a patient to sign-in
	* Also reject a patient, if not want to approve it.
	* Similar to admit a patient, Admin can also discharge a patient who was admitted.

Apart from above permissions for admin, he can generate invoice and can download the generated invoice. Generating invoice can be based on medical cost, room charge, doctor charge and other charges. In addition to this, admin can book, view and approve an appointment for a patient.
