*don't use "-k" to apply. because it can cause errors. And this can only be used to "delete". and follow the steps below.

follow these steps:


1.apply this file "secret-mysql-wp.yaml".

2.apply this file "pvc-mysql-wp.yaml".

3.then "describe" the file above. if it's still pending with the statement "fisrt ... " it means it's safe. And do the next step.

4.apply this file "deploy-wp-mysql.yaml".

5.do "exec" in this pod. Then go to "mysql -u root -p***" #hint : base64, create a database with the name "wordpress".

6.apply this file "pvc-wp.yaml".

7.do like step 3.

8.apply this file "deploy-wp.yaml".

9.get service and then acces the external port.
