## Network Hardening

Task 1  Patch the Linux Instances (Default Baseline)

Open Systems Manager → Fleet Manager and check that the Linux instances are visible (they’re already hooked up with the right IAM role).
Go to Patch Manager and start a Patch now job using the default Amazon Linux 2 baseline.
Set it to scan and install, allow reboot, and target instances using the Patch Group = LinuxProd tag.
Run it and watch the patch job finish for all three Linux instances.

<img width="1365" height="646" alt="Screenshot 2025-11-26 092006" src="https://github.com/user-attachments/assets/eb35a4d5-abe2-4a8c-98c4-c527609431ab" />


<img width="1365" height="647" alt="Screenshot 2025-11-26 093117" src="https://github.com/user-attachments/assets/327cfe7f-3a2e-43df-b282-ab6be761ff13" />
<img width="1365" height="647" alt="Screenshot 2025-11-26 100448" src="https://github.com/user-attachments/assets/4cfb05b4-4dba-47cd-bd29-af5dbddb7735" />
<img width="1365" height="646" alt="Screenshot 2025-11-26 102255" src="https://github.com/user-attachments/assets/68f08adf-7bd1-4bc0-864a-a6d5fc72c428" />
<img width="1365" height="642" alt="Screenshot 2025-11-26 103732" src="https://github.com/user-attachments/assets/31d6fc14-9446-42b6-a075-47c50953bd4f" />



Task 2  Create a Custom Windows Patch Baseline

Go back to Patch Manager and create a new baseline called WindowsServerSecurityUpdates for Windows.
Add two approval rules for Windows Server 2019: one for Critical security updates, one for Important ones, both auto-approving after 3 days.
Save the baseline and associate it with the WindowsProd patch group.

<img width="1365" height="645" alt="Screenshot 2025-11-26 103905" src="https://github.com/user-attachments/assets/44532844-8052-454b-8960-daf88a6f3035" />
<img width="1365" height="646" alt="Screenshot 2025-11-26 103803" src="https://github.com/user-attachments/assets/8a96d4be-f3e1-4572-80bb-8fceade5ad3b" />


Task 3  Patch the Windows Instances

Tag the three Windows EC2 instances with Patch Group = WindowsProd.
Return to Patch Manager, start another Patch now job, and target those tagged Windows instances.
Open the execution details once it starts and confirm that Run Command is applying the patches using your new patch baseline.

<img width="1365" height="639" alt="Screenshot 2025-11-26 104548" src="https://github.com/user-attachments/assets/d6dc1f80-88d7-40ef-9937-0bda34d6a572" />
<img width="1365" height="645" alt="Screenshot 2025-11-26 104700" src="https://github.com/user-attachments/assets/3dc6a9e5-7353-4b82-949f-5110d90f8485" />


<img width="1365" height="645" alt="Screenshot 2025-11-26 092815" src="https://github.com/user-attachments/assets/3d57b7d0-ca34-4bc6-8cf3-3a1a510bcb8f" />


Task 4  Verify Compliance

Back in Patch Manager, open the dashboard and check that all six instances show as compliant.
Use the Compliance Reporting view to confirm each instance’s status, last operation date, and the applied patches.
Open any Windows node to see the exact patches and install times.

<img width="1365" height="644" alt="Screenshot 2025-11-26 105843" src="https://github.com/user-attachments/assets/55b34963-b22f-4eac-be28-e18435cff9cf" />
<img width="1365" height="645" alt="Screenshot 2025-11-26 105857" src="https://github.com/user-attachments/assets/acafa675-a77c-45ce-9655-1260c94fa599" />





