# Challenge: Lock Out
## Author: r1c3t

- Challenge us the login.php page
<p align="center"><img src="./images/lockout1.png"></p>

- Use Burp Suite to see HTTP request. We will use the `Response to this request` feature to be able to modify the response from the request
<p align="center"><img src="./images/lockout2.png"></p>

- Edit status from 302 to 200 OK
<p align="center"><img src="./images/lockout3.png"></p>

- Then, the browser will render a new page, there is a PrintFlag button, we click on it to send a GET request to the server.
<p align="center"><img src="./images/lockout4.png"></p>

- Observing the returned payload we see the value of flag
<p align="center"><img src="./images/lockout5.png"></p>

## Flag is `gigem{if_i_cant_wear_croc_martins_to_industry_night_then_im_not_going}`