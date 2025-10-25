*A discussion about the Dybo project with Georges Khaznadar, an experienced French teacher in the field of sciences and computer deveployments in schools. April 2023*

***

## 1. Vision and Philosophy of the Dybo Project

| Key Idea | Details and Objectives |
| :--- | :--- |
| **Founding Philosophy** | Dybo is a **free nomadic computer system** (**hardware and software**), centered on the principle of **free software** whose source code is pushed to the end-user to encourage ownership. |
| **Educational Goal** | To replace the three main student supports: **books, notebooks, and binders**. |
| **Starting Point** | Development begins with the essential function of **handwritten note-taking** (to replace the notebook). |
| **Durability** | The hardware must be designed for a lifespan of **8 to 9 years**, covering the student's schooling from CM1/CM2 (4th/5th grade) to *Terminale* (last year of high school). |

***

## 2. Hardware and Technical Design (Hardware)

| Key Idea | Specifications and Justifications |
| :--- | :--- |
| **Physical Format** | A device the size of a **large notebook**, slightly larger than A4. |
| **Screens and Stylus** | **Two A4 screens** (or 14-15 inches) are necessary to allow students to work comfortably with **two documents simultaneously** (e.g., textbook and notebook). The use of a **stylus** is fundamental for handwritten note-taking. |
| **Ideal Weight** | Since Dybo replaces **8 to 10 kg** of school supplies, a weight of **3 or 4 kg** is considered acceptable. However, Georges suggests that **2.5 kg** would be more convincing to facilitate adoption and avoid it becoming a "potential barrier." |
| **Architecture** | The choice is for a **"free" RISC V** processor and a **Linux** operating system (ideally Framebuffer). |
| **Connectivity** | The device must be capable of managing **localized wireless connectivity** (see section 5) for autonomous classroom operation. |

***

## 3. Software and Educational Design

| Key Idea | Features and Concepts |
| :--- | :--- |
| **Educational Model** | Based on Alan Kay's concept of the **Computerized Knowledge Model** (*dynamic media*). |
| **The Digital Notebook** | The main software, **PaperMorph**, is the **backbone** simulating the student's notebook. It manages the insertion of **handwritten notes** and **dynamic media** (*Morphs*). |
| **Empowerment Through Free Software** | **Dynamic media** are provided via rich script libraries. They must be **easily modifiable** by novice teachers to promote skill development (linking to the free software philosophy). |
| **"Professional" Functions** | The software is designed for teaching practices: automatic opening of the **ad-hoc binder** based on the class schedule, proposal to automatically **schedule** a given assignment, and management of **PDF** documents with stylus annotation. |

***

## 4. Evaluation and Interactivity (AMC Scenario)

| Key Idea | Application and Advantages of Auto-Correction |
| :--- | :--- |
| **Software Link** | Dybo is well-suited for using the **Auto-Multiple-Choice (AMC)** software (maintained by Georges via a Debian package). |
| **Evaluation Scenario** | The teacher sends an **AMC** work document to the students via **local wave** (Wi-Fi/Bluetooth). |
| **Instant Correction** | Students complete and return the document to the teacher, whose Dybo **automatically corrects** it, records the grade, and sends the corrected work back to the student, all in **less than 15 seconds**. |
| **Advantages** | The electronic exchange enables pedagogical interactions impossible with paper (e.g., randomized multiple-choice questions) and the scenario **eliminates the need for photocopying and scanning** for evaluation. |

***

## 5. Connectivity and Deployment Challenges

| Key Idea | Issues Raised and Dybo Solutions |
| :--- | :--- |
| **Institutional Wi-Fi Network** | The observation is the **poor quality and unreliability** of institutional Wi-Fi networks (AP/Radius issues) which led to the failure of past tech rollouts. |
| **Dybo Solution (Autonomy)** | In-class use **must not require remote authentication**. Document sharing occurs **locally in class peer-to-peer** via **Bluetooth and/or Wi-Fi** from the teacher's Dynabook. A **local Wi-Fi network is the right solution** in most cases. |
| **Adoption Strategy** | The approach must be **humble** and allow Dybo to **coexist with traditional uses**. The user must derive a **visible and measurable individual benefit**. |
| **Deployment Scenarios** | **"Top-Down" Approach** (entire establishment requiring "credible political will") or **"Bottom-Up" Approach** (small pedagogical team in an ordinary establishment, judged more frequent). |
| **Institutional Obstacles** | The French system is considered **self-blocking** due to the "administrative and pedagogical layers" (*mille-feuille*), friction between hardware prescribers and pedagogical prescribers, and the prohibition for the national publisher (CNDP) to publish textbooks. |
```
