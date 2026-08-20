# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: LAKSHMIDHAR N
* **Register Number**: 212224230138
* **Date of Submission**: 20.08.2026

---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Workflow (Student Explanation)



Attached the EBS volume to the EC2 instance and checked the available storage.

Created an ext3 file system on the new volume and mounted it at /mnt/data-store.

Created a file on the volume, added text to it, and verified the data.

Created an EBS snapshot, deleted the original file, and created a new volume from the snapshot.

Attached and mounted the restored volume at /mnt/data-store2 and verified that file.txt was successfully restored.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1917" height="916" alt="image" src="https://github.com/user-attachments/assets/677ea035-9094-4b7b-be8d-53bde3cdec58" />



---

### Screenshot 2: EBS Volume Attached to EC2

  <img width="1914" height="857" alt="image" src="https://github.com/user-attachments/assets/b653476b-8f28-456f-9baf-4f2876ac4c03" />


---

  ### Screenshot 3: Mounted Volume with Data

<img width="1443" height="714" alt="image" src="https://github.com/user-attachments/assets/38b33b32-08d4-4e72-b40b-2ec117b3ed37" />


---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
