# Animix telegram miniapp bot
![banner](img/image.png)

This script automates various tasks for the Animix miniapp telegram.

## Features

- **Auto Join/Claim Missions**
- **Auto Gatcha New Pets**
- **Auto Complete Quests**
- **Auto Merge Pets**
- **Auto Claim Rewards**
- **Support Multy accounts**
- **Support Proxy Usage**

## Prerequisites

- Node.js installed on your machine
- `users.txt` file containing user data follow instruction below to get:
- log in to your telegram on pc
- Open Animix miniapp telegram https://t.me/animix_game_bot?startapp=KRTIRBzDfsrq
- inspect or just F12 find application
- in session storage find `tgWebAppData` and copy all value. `user=....`
![usersData](img/image-1.png)

- if yours starts with "query_.sdjydh" copy from query till the end of the line and paste in users.txt
<img width="626" alt="image" src="https://github.com/user-attachments/assets/35fc5621-2361-4c26-894a-adfd515c4127" />


## Run on mobile with Termux
- download termux on playstore
- run the following commands to install Ubuntu

```shell
apt upgrade && apt update
apt update
```


```sh
apt install proot-distro
proot-distro install ubuntu
```
- you may need to quit termux and close the app from background before proceeding

```sh
proot-distro login ubuntu
```

<img width="427" alt="image" src="https://github.com/user-attachments/assets/91133f5f-07d1-4518-90ce-aa71cf19d5ec" />

```sh
apt update && apt upgrade -y 
apt install sudo nano adduser
adduser intellygentle
```

<img width="345" alt="image" src="https://github.com/user-attachments/assets/de4c5cab-6b68-42e1-8503-1c12c6c49752" />

```sh
nano /etc/sudoers
```
![image](https://github.com/user-attachments/assets/b1a46e5c-fdd7-45d0-8379-8f2ac0bfdd3f)

```sh
usermod -aG sudo intellygentle
su - intellygentle
```

- full X thread on how to install ubuntu on termux
https://x.com/Intellygentle/status/1866529976964812874

## Installation

1. Clone the repository:
    ```sh
    https://github.com/intellygentle/animixBot.git
    cd animixBot
    ```

2. Install the required dependencies:
    ```sh
    npm install
    ```
3. Input your user data in `users.txt` file, one user per line; You will get it by loging in your tg on a pc. You can see the example above 
    ```sh
    nano users.txt
    ```


4. Run the script:
    ```sh
    npm run start
    ```

## ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

This project is licensed under the [MIT License](LICENSE).
