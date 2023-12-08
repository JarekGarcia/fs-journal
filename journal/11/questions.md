# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | extends a class with properties of another class to be used on one class |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | Yes the class inherits all or selected properties from the base class so you can reuse certain classes to extend other classes a nice reusable function. |

3. How does ***accessibility*** affect inheritance?

  > | Well it depends on the access type of the class if it is public it will be accessible but if it is a private class it won't be accessible. |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | Only one property can be a primary key on a table and usually it is the id and it creates a unique index for each object inserted into the table and the foreign key is a property referenced in another table. |

5. What is an ***alias***?

  > | an alias is a way to shorten a namespace or type so you don't have to type the complete name or type out speeds of coding a bit. |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > | SELECT * FROM patient_doctors WHERE patient_doctors.doctorId = 1 |

    this will pull out all the patients for the doctor with the id of 1...

    alternative answer would be just in case you needed this version:
    internal List<Patient> GetPatientsByDoctorId(int doctorId)
    {
    string sql = @"
    SELECT 
    pats.*, 
    patdocs.*
    FROM patients pats
    JOIN patient_doctors patdocs ON pats.id = patdocs.patientId
    WHERE patdocs.doctorId = @doctorId;";

     List<Patient> patients = _db.Query<Patient, Patient_Doctor, Patient>(sql, (patients, patient_doctors) =>
         {
            return patients;
         }, new { doctorId }).ToList();
        return patients;

    }



    which uses a join statement so idk hopefully one of these answers is what the question is asking for.
