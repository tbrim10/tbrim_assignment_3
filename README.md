#Personal Information Storage (strings)
full_name = 'Takiya Brim'
Student_email = 'tjbrim@aggies.ncat.edu'
Hometown = 'Martinsville,Va'
Graduating_semester = 'Spring 2028'
Major = 'Computer Science'

# Academic Data (lists)
Current_courses = ['COMP 163','MATH 131','LIBS 202','HIST 207''SPCH 250']
Completed_courses = []
Credit_hours = [3, 4, 3, 3, 3] # corresponding to current courses
Gpa_history = [] #semester GPAs as floats

# Contact Information Storage (tuples)
emergency_contact = ('Mom','Ebony Horne','276-123-4567')
home_address = ('P. Sherman', '42 Wallaby Way', 'Sydney','28202')
instagram_info = ('Instagram', '@t2smoovee._', 979)
twitter_info = ('Twitter', '', )
birtday = ('Birthday', '10', '29', '2004')

# Interest Tracking (sets)
current_skills = {'Cooking', 'Basic car knowledge'}
skills_to_learn = {'Python', 'Data structures', 'Git','Public speaking'}
career_interest = {'Architectural Engineering','Civil Engineering'}
hobbies = {'Gaming', 'Photography', 'Fishing', 'Hunting', ,Drawing','Reading', 'Soccer', 'Music'}
entertainment_backlog = {'The First to die at the end','College football 26'}

#Organizational Mapping (dictionaries)
course_credits = {'COMP 163': 3, 'MATH 131': 4, 'LIBS 202': 3, 'HIST 207': 3, 'SPCH 250': 3}
course_professors = {'COMP 163': 'Prof. Rhodes', 'MATH 131': 'Dr.Chen', 'LIBS 202': 'Prof Cody', 'HIST 207': 'Prof Beale', 'SPCH 250': 'Prof Jones'}
course_rooms = {'COMP 163': 'Gibbs 337', 'MATH 131': 'Marteena 214', 'LIBS 202': 'GCB 306', 'HIST 207': 'Gibbs 107','SPCH 250':'Online'}
monthly_budget = {'Food': 175, 'Entertainment': 50, 'Books': 70, 'Transportation': 60}
study_hours_per_subject = {'Programming': 2, 'Math': 2, 'Libs: 1, 'History': 3, 'Speech':0}
contact_directory = {'Mom': '123-456-7895', 'Roommate': '456-789-1290', 'Academic Advisor': '336-678-0092'}

#Calculations
total_credits = sum(Credit_hours)
cumulative_gpa = sum(Gpa_history) / len(Gpa_history)
completed_courses_count = len(Completed_courses)
total_study_hours = study_hours_per_subject['Programming'] + study_hours_per_subject['Math'] + study_hours_per_subject['English'] + study_hours_per_subject['History']
academic_load = total_credits + total_study_hours
total_monthly_budget = monthly_budget['Food'] + monthly_budget['Entertainment'] + monthly_budget['Books'] + monthly_budget['Transportation']
daily_food_budgget = monthly_budget['Food'] / 30
annual_budget = total_monthly_budget * 12
study_cost_per_hour = monthly_budget['Books'] / total_study_hours

#Analytics Calculations
total_media_followers = instagram_info[2] + twitter_info[2]
skills_comparison = len(current_skills) / len(skills_to_learn)
entertainment_backlog_count = len(entertainment_backlog)

print("=" * 64)
print("              PERSONAL ACADEMIC & LIFE PORTFOLIO")
print("=" * 64)

# Print Personal Information section
print(f"Student: {full_name} | Email: {Student_email}")
print(f"From: {Hometown} | Graduating: {Graduating_semester}")
print(f"Major: {Major}")
print()

print("=== ACADEMIC PROFILE ===")
# Use f-strings and round() for clean decimal display
print(f"Current Semester: {total_credits} credits across {len(Credit_hours)} courses")
print(f"Cumulative GPA: {round(cumulative_gpa, 2)}")
print(f"Weekly Study Time: {total_study_hours} hours")
print(f"Academic Investment: ${round(study_cost_per_hour, 2)} per study hour")
print()

print("Current Courses:")
# Access list and dictionary elements by index and key
print(f"{Current_courses[0]} - {course_credits[Current_courses[0]]} credits - {course_professors[Current_courses[0]]} - {course_rooms[Current_courses[0]]}")
print(f"{Current_courses[1]} - {course_credits[Current_courses[1]]} credits - {course_professors[Current_courses[1]]} - {course_rooms[Current_courses[1]]}")
print(f"{Current_courses[2]} - {course_credits[Current_courses[2]]} credits - {course_professors[Current_courses[2]]} - {course_rooms[Current_courses[2]]}")
print(f"{Current_courses[3]} - {course_credits[Current_courses[3]]} credits - {course_professors[Current_courses[3]]} - {course_rooms[Current_courses[3]]}")
print()

# Print Personal Development section
print("=== PERSONAL DEVELOPMENT ===")
# Print sets as they are, which will display the elements
print(f"Current Skills: {current_skills}")
print(f"Learning Goals: {skills_to_learn}")
print(f"Career Interests: {career_interest}")
# Use len() to count elements in the sets
print(f"Skills Currently Have: {len(current_skills)}")
print(f"Skills Want to Learn: {len(skills_to_learn)}")
print()

# Print Financial Overview section
print("=== FINANCIAL OVERVIEW ===")
# Use dictionary key access and multiplication
print(f"Monthly Budget: ${total_monthly_budget}")
print(f"Food: ${monthly_budget['Food']} (${round(daily_food_budgget, 1)}/day)")
print(f"Entertainment: ${monthly_budget['Entertainment']}")
print(f"Books: ${monthly_budget['Books']}")
print(f"Transportation: ${monthly_budget['Transportation']}")
print(f"Annual Projection: ${annual_budget}")
print()

# Print Connections & Contacts section
print("=== CONNECTIONS & CONTACTS ===")
# Access tuple elements by index
print(f"Emergency Contact: {emergency_contact[1]} ({emergency_contact[0]}) - {emergency_contact[2]}")
print(f"Home Address: {home_address[0]}, {home_address[1]}, {home_address[2]} {home_address[3]}")
# Print the calculated total followers and platform count
print(f"Social Media Presence: {total_media_followers} followers across 2 platforms")
print(f"Key Contacts: {len(contact_directory)} people in directory")
print()

# Print Life Statistics section
print("=== LIFE STATISTICS ===")
print(f"Total Courses Completed: {completed_courses_count}")
print(f"Current Academic Load: {academic_load} weekly commitments")
print(f"Entertainment Backlog: {entertainment_backlog_count} items")
print(f"Current Hobbies: {len(hobbies)} activities")

# Print the footer
print('=' * 64)
