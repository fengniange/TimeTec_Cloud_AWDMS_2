# TimeTec_Cloud_AWDMS_2(Storage XSS)

NAME OF AFFECTED PRODUCT： AWDMS

AFFECTED AND： 2.0

Description : The TimeTec AWDMS is an online application that offers Application Programming Interface (API) for third-party application developers to integrate with TimeTec terminals; to retrieve user information, biometric data, transaction logs, and TimeTec devices information.



Description of vulnerability : I found a stored XSS vulnerability after logging in to the system,But this time it comes from the name parameter


Affected Webpage : Backend page


Step 1 : Find the website and log in using the weak password admin/admin.
The website title is "TimeTec Cloud AWDMS", which is the characteristic of his website.
![img.png](1.png)

Step 2 : Find the Zone in the advanced features, create a new one here and add our xss payload to trigger the storage vulnerability.
The padyload is `<img src=x onerror=alert(1)>`
![img.png](2.png)

Step3: Depart successfully after saving.
![img.png](3.png)




