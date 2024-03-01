# Challenge 6: Generate Scripts using GitHub Copilot - Solution Guide

## Task 1: Generate Sysadmin scripts

In this task, you'll utilize GitHub Copilot to generate sysadmin resource monitoring scripts for CPU and Memory usage for a Linux VM and disk usage for a Windows VM.

1. In your VS Code, ask the GitHub Copilot Chat to generate a sysadmin script that monitors CPU and Memory usage with a threshold limit for a Linux VM and copy the script in a new file.

   ![](/media/generate-bash-script.png)

1. You'll notice that the GitHub Copilot generates a bash script that monitors CPU and Memory usage for a certain threshold limit and also explains its usage.

1. Now, ask the GitHub Copilot Chat to generate a sysadmin script that monitors disk usage with a threshold limit for a Windows VM and copy the script in a new file.

   ![](/media/generate-ps-script.png)

1. You'll notice that the GitHub Copilot generates a powershell script that monitors disk usage for a certain threshold limit and also explains its usage.

## Task 2: Refactor or debug the generated scripts

In this task, you'll refactor/debug the sysadmin scripts generated by the GitHub Copilot in the previous task.

1. Select the entire script and click **Ctrl+Enter** to view the suggestions provided by GitHUb Copilot to refactor or debug the script.

1. **Accept** the best suitable suggestions to fix the scripts.

1. You can also utilize GitHub Copilot Inline Chat to command the GitHub Copilot to enhance and fix the scripts.

1. Save the files after you have successfully utilized the GitHub Copilot to refactor and fix the scripts.

   - Bask script to monitor CPU and Memory usage in a Linux VM.
     ```
     #!/bin/bash

     # Sysadmin Resource Monitoring Script

     # Set the thresholds for CPU and memory usage (in percentage)
     cpu_threshold=90
     memory_threshold=90

     # Get the current CPU usage
     cpu_usage=$(top -bn1 | grep "Cpu(s)" | awk '{print $2}' | cut -d'%' -f1)

     # Get the current memory usage
     memory_usage=$(free | grep Mem | awk '{print $3/$2 * 100.0}' | cut -d'.' -f1)

     # Check CPU usage
     if [ "$cpu_usage" -gt "$cpu_threshold" ]; then
         # CPU usage exceeds the threshold, send an alert
         echo "CPU usage is above the threshold: ${cpu_usage}%"
         # Add your alerting mechanism here (e.g., send an email, log to a file, etc.)
     else
         # CPU usage is within the acceptable range
         echo "CPU usage is within the acceptable range: ${cpu_usage}%"
     fi

     # Check memory usage
     if [ "$memory_usage" -gt "$memory_threshold" ]; then
         # Memory usage exceeds the threshold, send an alert
         echo "Memory usage is above the threshold: ${memory_usage}%"
         # Add your alerting mechanism here (e.g., send an email, log to a file, etc.)
     else
         # Memory usage is within the acceptable range
         echo "Memory usage is within the acceptable range: ${memory_usage}%"
     fi
     ```
   - PowerShell script to monitor disk usage in a Windows VM
     ```
     # Sysadmin Disk Space Monitoring Script

     # Set the threshold for disk space usage (in percentage)
     $threshold = 90

     # Get the current disk space usage for the C: drive
     $diskUsage = Get-WmiObject Win32_LogicalDisk -Filter "DeviceID='C:'" | Select-Object @{Name='FreeSpace';Expression={$_.FreeSpace}}, @{Name='Size';Expression={$_.Size}}

     # Calculate the percentage of free space
     $freeSpacePercentage = ($diskUsage.FreeSpace / $diskUsage.Size) * 100

     # Check if disk space usage exceeds the threshold
     if ($freeSpacePercentage -gt $threshold) {
         # Disk space usage exceeds the threshold, send an alert
         Write-Host "Disk space usage is above the threshold: $($freeSpacePercentage)%"
         # Add your alerting mechanism here (e.g., send an email, log to a file, etc.)
     } else {
         # Disk space usage is within the acceptable range
         Write-Host "Disk space usage is within the acceptable range: $($freeSpacePercentage)%"
     }
     ```
## Task 3: Execute the scripts

In this task, you'll execute the sysadmin scripts generated by the GitHub Copilot in both Linux and Windows VMs.

1. Open command prompt and login to your Linux VM.

   > **Note:** Enter your Linux VM's admin username, password and Public IP Address.

1. Execute each command in from your bash script which monitors CPU and Memory usage and verify the results.

   ![](/media/execute-bash-script.png)

1. Open PowerShell ISE as an administrator, copy and paste the powershell script which monitors disk usage in a new file, run the script and verify the results.

   ![](/media/execute-ps-script.png)

   