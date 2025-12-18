<p align="center">
<img src="https://i.imgur.com/LKNiArP.jpeg" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Creating Virtual Machines with Azure</h1>
In this tutorial, we will walk through setting up a Windows and Linux virtual machine in Azure.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)

<h2>Operating Systems Used </h2>

- Windows 10 Enterprise, version 22H2 - x64 Gen2
- Ubuntu Server 22.04 LTS - x64 Gen2

<h2>High-Level Configuration Steps</h2>

- Step 1 - Create a Resource Group
- Step 2 - Create a Windows 10 or 11 Virtual Machine
- Step 3 - Create a Linux (Ubuntu) Virtual Machine
- Step 4 - Ensure both VMs are in the same Virtual Network / Subnet
- Step 5 - Task Complete 


<h2>Configuration Steps</h2>


<p>
<img width="860" height="750" alt="create RG 1_2" src="https://github.com/user-attachments/assets/abfbf701-9147-4adb-8636-245de179dec9" />
<img width="788" height="430" alt="create_resource_group" src="https://github.com/user-attachments/assets/03acbd25-2378-4a34-a04b-a2cecd4a0b04" />
</p>
<p>
Let's start with creating our Resource Groups. In the Azure portal, type resource group in the search bar and select Resource Group from the results. Click on Create. Name the group and select the Region. Click "Review + Create" to Finish.
</p>
<br />

<p>
<img width="1330" height="733" alt="create vm shot" src="https://github.com/user-attachments/assets/cf0c503a-931f-40c1-97ee-f152098a7757" />
</p>
<p>
Now let's create the Windows Virtual Machine. In the Azure portal, type Virtual Machine in the search bar and select Virtual Machine from the results.
</p>
<br />

<p>
<img width="805" height="874" alt="vm1" src="https://github.com/user-attachments/assets/9a5868a3-731c-4758-8f71-cc09567c68f4" />
</p>
<p>
Select the Resource Group that you created, name the VM, choose the same region as the Resource Group, and select a Windows Pro or higher version. In this example, we used Windows 10 Enterprise, version 22H2 - x64 Gen2.
</p>
<br />

<p>
<img width="828" height="684" alt="vm2" src="https://github.com/user-attachments/assets/85ce4a59-4239-4747-ad39-4060040ffbb2" />
</p>
<p>
Select a Disk Size with a minimum of 2 CPU and 8 GB memory. Create a Username and Password. Important: Check the Licensing box at the bottom. Click next until the Networking page.
</p>
<br />

<p>
<img width="1896" height="943" alt="vm3" src="https://github.com/user-attachments/assets/a8ba0cb9-f2ad-4b2f-8408-23aed572ba9c" />
<img width="855" height="867" alt="vm8_final create" src="https://github.com/user-attachments/assets/baa3c557-bf84-4730-b627-ba058acb02ac" />
</p>
<p>
In the Virtual Network section, Select Create New, name the VM, and select OK. Click Review + Create. If Validation passes on the next page, select Create.
</p>
<br />

<p>
<img width="935" height="615" alt="vm4" src="https://github.com/user-attachments/assets/8f51620f-7ad9-4e23-b836-336b7222ec5f" />
</p>
<p>
Time to create the Ubuntu(Linux) VM. In the Azure portal, type Virtual Machine in the search bar and select Virtual Machine from the results. Then select Create, then Virtual Machine.
</p>
<br />

<p>
<img width="818" height="831" alt="vm5" src="https://github.com/user-attachments/assets/7733f374-b3ea-47ff-91e5-bf4a8e51704d" />
</p>
<p>
Select the Resource Group that you created, name the VM, choose the same region as the Resource Group, and select an Ubuntu Server. In this example, we used Ubuntu Server 22.04 LTS - x64 Gen2.
</p>
<br />

<p>
<img width="780" height="775" alt="vm6" src="https://github.com/user-attachments/assets/0d64886c-85fe-417b-9fbb-5d03813af4ac" />
</p>
<p>
Select a Disk Size with a minimum of 2 CPU and 8 GB memory. For Authentication Type, choose Password, and create a Username and Password. Click next until the Network section.
</p>
<br />

<p>
<img width="844" height="814" alt="vm7" src="https://github.com/user-attachments/assets/d8192e89-e665-4743-9597-adf2f08fda6c" />
<img width="855" height="867" alt="vm8_final create" src="https://github.com/user-attachments/assets/a2cb5089-427b-4674-b28f-19b6c6094b21" />
</p>
<p>
Select the Virtual Network drop-down and select the new Vnet that you created. Select Review + Create. If Validation passes, select Create to finish.
</p>
<br />

<p>
<img width="1278" height="837" alt="vm9" src="https://github.com/user-attachments/assets/c396b643-6bbe-4fbd-b0c0-6733167a639f" />
</p>
<p>
Important: Within the Azure portal, verify that the Virtual network/subnet on the Windows and Ubuntu VMs are the same.
</p>
<br />

