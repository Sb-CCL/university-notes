
# **Lab Guide: Spot Speed Study for Pedestrian Safety Assessment**

#### **1. Purpose and Expectations**

**Purpose of this Lab:**
Team's objective is to perform a **Spot Speed Study** on a section of E Spring Avenue near Davidson Hall. The goal is to collect and analyze vehicle speed data to assess whether the posted speed limit is appropriate for ensuring pedestrian safety. You will apply statistical methods to your data, interpret the results, and communicate your findings and recommendations in a professional manner.

**What is Expected of You and Your Team:**
*   **Collaboration:** Work effectively in a team to collect accurate data.
*   **Analysis:** Use spreadsheet software (like Excel or Google Sheets) to perform statistical calculations on the collected data.
*   **Critical Thinking:** Evaluate the quality of your data, identify potential errors, and propose improvements to the study methodology.
*   **Professional Communication:** Individually synthesize the team's work into a formal email report addressed to a city official, demonstrating your ability to communicate technical information clearly and persuasively.

**Final Deliverable:**
Each team member must individually submit a **Formal Email as a PDF** addressed to Sam Fakename, City State Traffic Management Director. This email must contain your analysis, answers to all lab questions, and recommendations.

---

#### **2. Team Development Process: A Step-by-Step Guide**

Follow these phases to complete the lab correctly and efficiently.

##### **Phase 1: Team Setup and Data Collection (Procedure Steps 1-5)**

*   **Instruction 1: Form Teams**
    *   Divide your 4-person team into two pairs (Team A and Team B).
    *   Each pair will be assigned a different video clip to analyze.

*   **Instruction 2: Collect Data from Videos**
    *   **Roles for each pair:**
        *   **Person 1 (Caller):** Opens the video clip. For each vehicle, you will:
            1.  Call out the vehicle description (e.g., "blue sedan").
            2.  Call out the exact time the vehicle's front bumper crosses the **first orange dashed line** (start of the 150-foot speed trap).
            3.  Call out the exact time the vehicle's front bumper crosses the **second orange dashed line** (end of the speed trap).
        *   **Person 2 (Recorder):** Records the information called out by Person 1 on the **Spot Speed Lab Field Sheet**. You will calculate the time it takes to cover the 150-foot distance.
    *   **Switching Roles:** After recording data for 10 vehicles, the Caller and Recorder must switch roles. This ensures everyone participates equally. Each pair is responsible for recording 20 vehicles (10 per person).

*   **Instruction 3: Calculate Speeds**
    *   For each vehicle, calculate the time taken to travel the 150-foot distance: `Exit Time - Entry Time`.
    *   Calculate the speed in miles per hour (mph). The formula is:
        `Speed (mph) = (Distance in miles) / (Time in hours)`
        A more practical formula using feet and seconds is:
        **`Speed (mph) = (150 ft / Time in seconds) * (3600 sec/hr / 5280 ft/mile) ≈ (150 / Time_s) * 0.6818`**
    *   **Tip:** Set up your field sheet in a spreadsheet to do this calculation automatically.

*   **Instruction 4: Consolidate and Record Metadata**
    *   Combine the data from both pairs (Team A and Team B) into a single master list of 40 vehicles.
    *   **Crucially,** record all metadata on your field sheet:
        *   Date
        *   Time of data collection (from the video)
        *   Location (E Spring Ave near Davidson Hall)
        *   Weather Conditions (observed from the video)
        *   Road Conditions (e.g., dry, wet)
        *   Posted Speed Limit (you will need to find this from the lab materials or figure)

*   **Instruction 5: Create a Frequency Distribution Table**
    *   Organize your 40 speed values into a table with speed groups (e.g., 20-21 mph, 21-22 mph, etc.), similar to Figure 3 in the lab manual.
    *   Use tally marks to count how many vehicles fall into each speed group. This is your frequency distribution.

##### **Phase 2: Data Analysis in a Spreadsheet (Analysis Tasks 6-9)**

*   **Instruction 6: Tidy Your Data Table**
    *   Create a spreadsheet with columns for: Speed Group, Lower Limit (mph), Upper Limit (mph), Frequency (number of vehicles).
    *   **Remove empty rows** at the top and bottom of your speed groups, leaving only one row with a frequency of `0` at each end. This makes the table cleaner for reporting.

*   **Instruction 7: Save the Edited Table**
    *   This cleaned-up frequency table will be **Attachment 1** in your final email.

*   **Instruction 8: Calculate Relative Frequency (Column E)**
    *   **Definition:** Relative Frequency = (Frequency of a speed group) / (Total number of vehicles) * 100%.
    *   **Formula Example:** If your frequency is in cell D2 and total vehicles (40) is in cell `$D$20`, the formula in E2 would be: `=(D2/$D$20)*100`.
    *   Use **absolute referencing** (`$D$20`) for the total so you can copy the formula down the column. Format the result to have one decimal place.

*   **Instruction 9: Calculate Cumulative Frequency (Column F)**
    *   **Definition:** Cumulative Frequency is the running total of the relative frequencies. It shows the percentage of vehicles traveling *at or below* a given speed.
    *   **Formula Example:** For the first data row (F2), it might just be `=E2`. For the next row (F3), the formula is `=F2+E3`. Copy this formula down the column.

##### **Phase 3: Interpretation and Report Writing (Questions 10-14)**

Answer these questions within the body of your formal email. **Define technical terms for your audience.**

*   **Guidance for Question 10 (Central Tendency):**
    *   **Define "Central Tendency":** Explain it means the data clusters around a central value, like the average (mean) or most frequent value (mode).
    *   **Answer:** Look at your frequency distribution chart. Does it have a clear peak? If the vehicles' speeds are mostly grouped around a specific value (e.g., most cars were going between 32-38 mph), then your data exhibits central tendency. If the speeds are spread out evenly with no clear peak, it does not.

*   **Guidance for Question 11 (Comparison to Posted Limit):**
    *   Calculate the **mean (average)** and **85th percentile speed** (the speed at which 85% of drivers are traveling at or below). The 85th percentile is often used by engineers to set rational speed limits.
    *   Compare these values to the posted speed limit. Are most drivers exceeding the limit? If so, this indicates a potential safety risk for pedestrians and may suggest the limit is set unrealistically low.

*   **Guidance for Questions 12-14 (Validity and Error):**
    *   **Q12: Circumstances:** Did weather, time of day, or visible pedestrians in the video influence driver behavior?
    *   **Q13: Sources of Error:**
        1.  **Human Reaction Time Error:** Slight delays in starting/stopping the timer. This affects individual speed calculations.
        2.  **Small Sample Size:** 40 vehicles may not perfectly represent all traffic at that location.
        3.  **Measurement Error:** Difficulty in precisely identifying when a car crosses the line on a video.
    *   **Q14: Proposed Changes & $350 Grant:**
        *   **For Reaction Time:** Propose using automated timing gates. With $350, you could purchase a **radar gun** (~$150-$300) to measure speed directly and eliminate timing errors.
        *   **For Sample Size:** Propose collecting data over multiple days and times. The grant money could fund a **simple traffic counter** or be used as a stipend for more data collection hours.
        *   **For Measurement Precision:** Using higher-resolution cameras or on-site measurement with calibrated equipment would help. Cite a source for the equipment you choose (e.g., "According to Eno Center for Transportation, radar guns are the standard for accurate spot speed studies.").

---

#### **3. Lab Procedure Checklist**

Use this checklist to ensure you complete all required steps.

**Phase 1: Data Collection**
- [ ] Teams divided into pairs.
- [ ] Roles (Caller/Recorder) assigned and switched after 10 vehicles.
- [ ] 40 vehicle speeds accurately recorded and calculated.
- [ ] All metadata (date, weather, location, speed limit) recorded.
- [ ] Frequency distribution table with tally marks completed.

**Phase 2: Data Analysis**
- [ ] Data entered into a spreadsheet.
- [ ] Frequency table tidied (empty rows removed).
- [ ] Relative Frequency calculated correctly (Column E).
- [ ] Cumulative Frequency calculated correctly (Column F).
- [ ] Cleaned data table saved for attachment.

**Phase 3: Report Writing**
- [ ] Formal email drafted in a professional tone.
- [ ] Questions 10-14 are answered thoroughly and clearly.
- [ ] Terms "central tendency" and "dispersion" are defined.
- [ ] Analysis includes mean and 85th percentile speed.
- [ ] Recommendations about the speed limit's efficacy are made.
- [ ] Equipment proposals for the grant are specific and justified with citations.
- [ ] Data table is attached at the end of the PDF document.
- [ ] Final email is exported as a PDF and submitted.

By following this guide, your team will systematically work through the lab, ensuring accurate data collection, robust analysis, and a professional final deliverable. Good luck