
# user registration system

a simple registration system using php and mysql



## Features:

- login/logout (sign-in), session- or token-based
- user profile (retrieving / updating)
- Views can be authenticated via session or auth token
- reset password
- Supports only one email per user (as model field)
- compatible with both mobile and desktop view(completly responsive)
- change password


## Installation & Configuration


Clone the project

```bash
 git clone:https://github.com/SamhithMR/User-Registration.git
```

(run below commands in sql query section)         
-  create a database named "user_registration" 
 
```bash
 CREATE DATABASE user_registration;  
```
 - creat table named `tbl_member` in user_registration database

```bash
CREATE TABLE `tbl_member` (
  `id` int(11) NOT NULL,
  `username` varchar(255) NOT NULL,
  `password` varchar(200) NOT NULL,
  `email` varchar(255) NOT NULL,
  `create_at` timestamp NOT NULL DEFAULT current_timestamp() ON UPDATE current_timestamp()) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```
- Indexes for table `tbl_member`

```bash
ALTER TABLE `tbl_member`
  ADD PRIMARY KEY (`id`);
```

- auto_increment for table `tbl_member`
```bash
ALTER TABLE `tbl_member`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=5;
COMMIT;
```
Now you can continue by starting MySql and apache server at
```bash
127.0.0.1/user-registration
```



## Screenshots

![preview](https://github.com/SamhithMR/user-registration/blob/main/assets/preview.png)

