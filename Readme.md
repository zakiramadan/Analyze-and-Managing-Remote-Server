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

1. **Activate and Access Web Console**

   - Install Cockpit if not installed already.

   ```bash
    sudo dnf install cockpit
   ```

   - Enable and start the cockpit service.

   ```bash
    sudo systemctl enable --now cockpit.socket
   ```

   - Add the cockpit service to the firewall.

   ```bash
    sudo firewall-cmd --add-service=cockpit --permanent
    sudo firewall-cmd --reload
   ```

2. **Mengakses Konsol Web**

- Open a web browser and navigate to https://servera.lab.example.com:9090.
- Log in with your username and password.

3. **Mengubah Kata Sandi di Konsol Web**

- Click the Accounts button in the navigation bar.
- Click your account label and then click the Set password button.
- Enter your old and new passwords, then click Set password.

4. **Jalankan Perintah dari Sesi Terminal**

- Click the Terminal button in the navigation bar to access the terminal.
- Verify command execution by running id command.

5. **Mengelola Layanan Sistem dengan Konsol Web**

- Start, enable, disable, and stop services from the Services section.
- Configure network interfaces and firewall rules from the Networking section.
- Administer user accounts from the Accounts section.

## Penilaian

- The instructions for activating and accessing the Web Console are clear and easy to follow.
- Instructions for changing passwords, running commands from a terminal session, and managing system services with the Web Console are also well presented.
- The included references provide additional resources for users to get further information.

## Catatan Tambahan

- Make sure to follow the steps carefully and understand each step before proceeding.
- If encountering difficulties, do not hesitate to refer to the references or ask for assistance from the instructor.
- After completing the exercise, take time to reflect on your experience and note down the things you have learned.
- This exercise is an opportunity to enhance practical skills in system administration, so make the most out of it.
