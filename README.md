# Optimization-Based-Automation-Scheduling-via-Mathematical-Modeling
--------------------------

### Notes: The following cases were developed from assumed scenarios and serve as dummy cases for demonstration purposes.

---
Problem Statement:

There are 45 employees working as production operators to produce lamp. Each day, the company has a production target that is divided between weekdays and weekends with the following details:
  - The target on weekday is to complete 6000 units.
  - The target on weekend is to complete 5000 units.

Based on this information, each operator has the same individual daily target which is to complete 200 units per day, in accordance with the company’s established standards. This target is essential to ensure the achievement of the overall daily production output.

However, the process of creating work schedules is still done manually by the HR team and production supervisors using spreadsheets and conventional records. Since the scheduling is done manually and without a supporting system, the process becomes highly complex and prone to errors.

Therefore, the HR and production supervision teams require assistance in generating schedules automatically based on several constraints as follows:

- There are 3 shifts where each shift consists of 8 working hours.
  - Shift 1 = 07:00 - 15:00
  - Shift 2 = 12:00 - 20:00
  - Shift 3 = 16:00 - 24:00
- Each employee should work at least one shift per day and one shift per week.
- Each employee should work only for 5 days each week and should have 2 days week off.
- No employees should work more than 5 consecutive days during any period.
- If employees get night shift (shift 3), employees do not work in morning shift in the next day or in next shift.
- Employees can request annual leave for a reason.

These cases will generate a 35 day (5 week) schedule for each employee based on the constraints above

---

The model also incorporates binary decision variables (0/1), allowing the optimization process to enforce conditional scheduling rules while keeping the formulation linear.

---
Methodology:
- Install pulp library in your jupyter notebook
  <img width="682" height="197" alt="image" src="https://github.com/user-attachments/assets/118f74f7-82ee-40cc-ac34-a5d76e8e8338" />

- Convert the problem statement into mathematical equation

  <img width="465" height="52" alt="image" src="https://github.com/user-attachments/assets/9aa962aa-0d49-465b-977c-c06e03b373bd" />
  
  Use `minimum optimization method`

- The program is success if the status = "Optimal"

  <img width="225" height="93" alt="image" src="https://github.com/user-attachments/assets/dc095f91-5463-4950-94bf-429359bb0d6f" />

---

Overview of the results:

  <img width="228" height="279" alt="image" src="https://github.com/user-attachments/assets/9d94a5f5-cdd9-4809-b770-69beb9857d7e" />
  

<img width="250" height="271" alt="image" src="https://github.com/user-attachments/assets/93108d1b-0ad2-41b3-94d5-974c47d143e9" />


you can rename the column name such as date, days of the week and others based on your requirements

---
Tools:
- Jupyter Notebook / Google Colab
- Python
- PuLP
- Pandas
- Numpy
