---
id: "Introduction"
aliases:
  - "Threat Modeling"
  - "Database Security Threats"
tags: []
---

### Database Security Threats
+ **Excessive Privileges**          : Users are granted **too much permission**
+ **Legitimate Privilege Abuse**    : Users with proper permissions **abuse their privileges**
+ **Storage Media Exposure**        : Data is **stored on unencrypted media**
+ **The Human Factor**              : **Mistakes** made by users

### Threat Modeling
+ Figuring out how an attacker could attack a system
    1) **Gather Information**           : What is the system? What does it do?
    2) **Decompose App**                : Break the system into components
    3) **DFDs (Data Flow Diagrams)**	: How does data flow through the components?
    4) **Identify Risk Areas**          : What are the most vulnerable components?
    5) **Use Cases**                    : How would an attacker attack the system?
    6) **Attack Trees**                 : What are the steps an attacker would take?

### Preventive Techniques
+ Methods to **prevent potential attacks**
	1) **Least Privilege**              : Only give users **enough permission to complete their job**
	2) **Restrict Database Operations**	: **Restrict users** from performing certain operations
	3) **Check For Non-Compliance**     : Check for users who are **not following the policy**

### Detective Techniques
+ Methods to **detect potential progress**
    1) **Identify Footprints**			: **Monitor the logs** for suspicious activity
	2) **Maintain Detection Systems**	: Keep audit logs, IDS, and other detection systems **up to date**

### Access Controls & Data Security
1) **Discretionary Access Control** (DAC)	: Owner of an object decides who can access it
2) **Rule Based Access Control**	(RuBAC)	: Access is determined by a set of rules	(ex. Firewalls)
3) **Role Based Access Controls**	(RBAC)	: Access is determined by a user's role		(ex. Admin Role)
4) **Mandatory Access Control**		(MAC)	: Access is determined by the system		(ex. ATMs)
    1) **Bell La Padula Model (Confidentiality)**: No read up, no write down
        + **Simple Security Property**    : Cannot read files of permissions above your level
        + **Star Property**               : Cannot write to files of permissions below your level

    2) **Biba (Integrity)**: No read down, no write up
        + **Simple Integrity Property** : Cannot read files below your integrity level
        + **Star Integrity Property**   : Cannot write to files above your integrity level

    3) **Clark-Wilson Model (Integrity)**: Separation of duties
        + **Constrained Data Item (CDI)**               : Data that is protected by the system
        + **Unconstrained Data Item (UDI)**             : Data that is not protected by the system
        + **Integrity Verification Procedures (IVP)**   : Procedures to verify the integrity of CDIs
        + **Transformation Procedures (TP)**            : Functions to modify CDIs

    4) **Brewer & Nash Model / Chinese-Wall Model (Integrity)**: Prevents conflict of interest
        + **Conflict of Interest**  : When data from two or more competing companies is accessed
        + **Chinese Wall Model**	: Prevents users from accessing data from competing companies

### Integrity Principles
1) **Goals of Integrity**
    1) Prevent **unauthorized users** from **modifying data**
    2) Prevent **authorized users** from **making invalid modifications to data**
    3) Maintaining **consistency** of data

2) **Consistency Integrity**    : Check if data is of proper format using checks
3) **Entity Integrity**		    : Data cannot have NULL values in primary key fields
4) **Referential Integrity**    : Foreign keys must reference a valid primary key
5) **Least Privilege**          : Users should only have enough permission to complete their job
6) **Granularity**              : Access controls should be as detailed as possible

7) **Well-Formed Transactions**: Transactions that follow the ACID principles
    1) **Atomicity**	: Either all transactions are performed or none are performed
    2) **Consistency**	: Data is consistent before and after the transaction
    3) **Isolation**	: Transactions are isolated from each other
    4) **Durability**	: Changes made by a transaction are permanent

8) **Constrains**: Rules that must be followed when inserting data into a database
    1) **NOT NULL Constraint**		: Fields cannot be NULL
    2) **Unique Constraint**		: Fields must be unique
    3) **Primary Key Constraint**	: Fields must be unique and not NULL
    4) **Foreign Key Constraint**	: Fields must reference a valid primary key
    5) **Check Constraint**         : Fields must be of a certain format (DATE, INT, etc.)
