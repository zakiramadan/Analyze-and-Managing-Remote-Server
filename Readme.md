# Panduan: Analyzing and Managing Remote Servers

## Tujuan

This exercise aims to provide practical understanding of how to analyze and manage remote servers using desktop Linux Ubuntu. Participants will use a series of commands and built-in tools to achieve this goal.

## Deskripsi

This exercise guides participants through the process of analyzing and managing remote servers using desktop Linux Ubuntu. Participants will use commands such as `ssh`, `ping`, `traceroute`, and `netstat` to check connectivity, trace packet routes, and evaluate the status of remote servers.

### Langkah-langkah

1. **Membuat Koneksi SSH ke Server Remote**

   - Use the `ssh` command to connect to the remote server.
     ```bash
     ssh username@remote_server_ip
     ```

2. **Memeriksa Konektivitas Jaringan**

   - Use the `ping` command to check connectivity with the remote server.
     ```bash
     ping remote_server_ip
     ```
   - Use the `traceroute` command to trace packet routes to the remote server.
     ```bash
     traceroute remote_server_ip
     ```

3. **Meninjau Status Port pada Server Remote**
   - Use the `netstat` command to view the status of ports on the remote server.
     ```bash
     netstat -tuln
     ```
   - Identify ports that are listening and the services running.

## Penilaian

- Success in establishing an SSH connection to the remote server.
- Ability to use the `ping` and `traceroute` commands to check network connectivity.
- Ability to use `netstat` to analyze port status on the remote server.
- Ability to analyze the information obtained and evaluate the status of the remote server.

## Catatan Tambahan

- Be sure to use commands carefully and only on servers you own or have appropriate permissions for.
- This exercise aims to provide practical understanding of analyzing and managing remote servers, which is an important skill in Linux system administration.
