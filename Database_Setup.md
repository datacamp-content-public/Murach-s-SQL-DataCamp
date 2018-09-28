### Step 1: Prepare your tables.

- [ ] Export the tables in your database(s) into separate .csv files
- [ ] In total, .csv files should be less than 10MB
- [ ] Upload your .csv files to the teach editor in the course-specs branch of your course.

### Step 2: Prepare your .sql file.

- [ ] Write a .sql file creating your database. See this example: https://assets.datacamp.com/production/repositories/3580/datasets/cf481971f9464bc87557cc9f2da5d45a126befd9/soccer_matches.sql
- [ ] Replace the links in the section "COPY <table> FROM ... " with the table links generated in the teach editor.
- [ ] Create one .sql file for all databases in your course.
- [ ] Upload your .sql file to the teach editor in the course-specs branch of your course.
     
### Step 3: Update your requirements.sh file.

- [ ] Update the requirements.sh file in the course-specs branch of your course on GitHub.
- [ ] Uncomment line 11 (wget ....) and replace the link with your .sql file link from the teach editor.
- [ ] Uncomment lines 13-16 and replace DATABASENAME with the name for your database from the .sql file in all places.
- [ ] Commit file directly to the course-specs branch on GitHub.

### Step 4: Setting up the pre-exercise code.

- [ ] In the teach editor, set up the following code:
     connect('postgresql', 'DATABASENAME')
     set_options(visible_tables = ['TABLE',  'TABLE'])
- [ ] Replace DATABASENAME with the database name from the requirements.sh file.
- [ ] Replace TABLE with 1 or more table names to be visible to students for an exercise. 
- [ ] Customize this code for every exercise.
