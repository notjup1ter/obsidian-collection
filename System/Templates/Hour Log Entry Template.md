<%*
// 1.list of work types 
const workTypes = ["Async work", "Meeting (Team)", "Meeting (Mentor)", "Meeting (1-1)", "Training (Workshop)", "Onboarding", "Async Communication", "Misc"]; 
// 2. Open the selection menu (Suggester) const 
selectedType = await tp.system.suggester(workTypes, workTypes, false, "Select what type of work is being logged"); 

// 3. If you cancel the menu (Esc), stop the script 
if (!selectedType) return; 
// 4. Get today's date 

const date = tp.date.now("YYYY-MM-DD");
// 5. Output the table row // Format: | Date | Type | Description | Hours | 
tR += `| ${date} | ${selectedType} | | |`;


%>
