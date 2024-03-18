# Analyze and Manage Remote Servers

## Introduction

This repository contains a guided exercise on how to analyze and manage remote servers using the web console on Red Hat Enterprise Linux. The exercise covers various tasks such as activating the web console, accessing it, changing passwords, running commands from terminal sessions, managing system services, and more.

## Tujuan

The purpose of this exercise is to provide users with the understanding and skills to use the Web Console to efficiently manage remote servers. By following this exercise, users are expected to be able to:

1. Understand how to activate and access the Web Console on Red Hat Enterprise Linux.
2. Able to manage system services, change passwords, and run commands from terminal sessions through the Web Console.
3. Manage user accounts and perform other administrative actions using the Web Console interface.
4. Learn how to identify and resolve issues through features in the Web Console such as monitoring the system, checking logs, and creating diagnostic reports.

## Petunjuk

Follow the steps below to complete the exercise:

1. **Open Lab Console Redhat dan mulai**

   ```bash
    lab start support-cockpit
   ```

   ![App Screenshot](</Image/1. lab start support-cockpit.png>)

   ```bash
    ssh student@servera
   ```

   ![App Screenshot](</Image/19. student@servera.png>)

   ```bash
    sudo systemctl enable --now cockpit.socket
   ```

   ![App Screenshot](</Image/2. systemctl enable --now cockpit.socket.png>)

2. **Kemudian buka browser firefox redhat anda dan ketik link berikut, kemudian scroll ke bawah dan klik `Accept and risk`**

- Open a web browser and navigate to https://servera.lab.example.com:9090 or IPAddress:9090

![App Screenshot](</Image/10. advanced.png>)

![App Screenshot](</Image/11. accept the risk and continue.png>)

3. **Login dengan akun berikut :**

- Username : student
- Password : student

![App Screenshot](</Image/13. user dn pwd=student.png>)

4. **Buka limit access atau untuk mengganti menjadi administrator.Klik `Turn on administrative access`**

![App Screenshot](</Image/15. turn on administrative access.png>)

5. **Klik `Authenticate`**

![App Screenshot](</Image/16. switch to administrative access.png>)

6. **Masuk ke Account >> Create New Account**

![App Screenshot](</Image/40. Existing user accounts.png>)

7. **Isi data akun**

- Full name: manager1
- Username: manager1
- Password: 01redhat78#
- Confirm: 01redhat78#

![App Screenshot](</Image/13. create new account.png>)

8. **Buka Terminal >> id manager1 >> sudo usermod -aG wheel manager1 >> id manager1**

![App Screenshot](</Image/14. command terminal.png>)

9. **Masuk ke Service >> cari filter dengan nama psacct, kemudian klik yang biru**

![App Screenshot](</Image/15. kernel process accounting.png>)

10. **Active kan server psacct.service**

![App Screenshot](</Image/16. klik tombol on kernel process.png>)

11. **Log out dan buka terminal, kemudian akhiri dengan perintah:**

- Log out

![App Screenshot](</Image/17. log out.png>)

```bash
 lab finish support-cockpit
```

![App Screenshot](</Image/18. lab finish support-cockpit.png>)

## Penilaian

- The instructions for activating and accessing the Web Console are clear and easy to follow.
- Instructions for changing passwords, running commands from a terminal session, and managing system services with the Web Console are also well presented.
- The included references provide additional resources for users to get further information.

## Catatan Tambahan

- Make sure to follow the steps carefully and understand each step before proceeding.
- If encountering difficulties, do not hesitate to refer to the references or ask for assistance from the instructor.
- After completing the exercise, take time to reflect on your experience and note down the things you have learned.
- This exercise is an opportunity to enhance practical skills in system administration, so make the most out of it.
