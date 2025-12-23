# Forensics

***

## The First Strike

* Provided PCAP can be opened using wireshark. 
* We can use `FTP` as a filter and go through different protocols to find multiple failed login attempts.

<img width="1302" height="114" alt="image" src="https://github.com/user-attachments/assets/aa9f638c-dc50-43b6-bd64-ec70882d88ad" />

* Using `frame contains "logged in"` helps us find our required login attempt.

<img width="1144" height="114" alt="image" src="https://github.com/user-attachments/assets/900bdf8e-fc3f-46fd-83ee-8493c42cd743" />


Flag : `csd{Elf67_snowball}`

***

## Syndiware

> Description

The Krampus Syndicate has never been subtle, but their newest initiative, codenamed Syndiware, might be their boldest misstep yet. Designed as a "consumer-friendly malware suite," Syndiware appears to target the youngest and most gullible users on the network: interns, seasonal hires, and anyone who believes free virtual currency generators are safe to run.

One such recruit learned this the hard way. Minutes after launching a suspicious executable, his entire workstation transformed into a theater of chaos: missing files, corrupted data structures, and a ransom note full of melodramatic threats. The intern claims he only clicked "Run Anyway" once. (The security logs suggest otherwise.)

What the Syndicate didn't expect is that this early build of Syndiware still has its rough edges and bugs. Somewhere in those remnants lies something important... something the Syndicate didn't intend for anyone to recover.

Follow the traces of the intrusion, work out the Syndicate’s techniques, and reveal the concealed Syndiware relic they attempted to hide.

File: [syndicate_locker.zip](https://github.com/h011o/madhav_phase2/blob/main/files/syndicate_locker.zip)

## Solve

Provided zip-file has a memory dump along with the encryption script used. Another folder called encryption_files has all the data in its encrypted format ending with `.enc`
