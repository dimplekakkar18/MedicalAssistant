Environment required to run the code:
your system must have the follwowing dependencies-
Flask==2.2.2
numpy==1.24.3
pandas==2.0.3
scikit-learn==1.3.0


Installation steps:
Clone this repository to your local machine using git clone https://github.com/dimplekakkar18/MedicalAssistant.git
Install the required dependencies by running pip install -r requirements.txt


To run the web application, execute the following command:
python main.py

This will start the Flask web server, and you can access the application by navigating to http://localhost:5000 in your web browser.

The application allows users to input their symptoms, get disease predictions, and receive recommendations for doctors specializing in the predicted diseases. Additionally, users can access detailed information about diseases, precautions, medications, workouts, and diets.

Please enter symptoms from the below list seperated by commas as the model is trained for these 132 symptoms. If you enter any other symptom or do spelling mistake- it will take you to the error page showing "symptom not recognized"

[itching, skin_rash, nodal_skin_eruptions, continuous_sneezing, shivering, chills, joint_pain, stomach_pain, acidity, ulcers_on_tongue, muscle_wasting, vomiting, burning_micturition, spotting_urination, fatigue, weight_gain, anxiety, cold_hands_and_feets, mood_swings, weight_loss, restlessness, lethargy, patches_in_throat, irregular_sugar_level, cough, high_fever, sunken_eyes, breathlessness, sweating, dehydration, indigestion, headache, yellowish_skin, dark_urine, nausea, loss_of_appetite, pain_behind_the_eyes, back_pain, constipation, abdominal_pain, diarrhoea, mild_fever, yellow_urine, yellowing_of_eyes, acute_liver_failure, fluid_overload, swelling_of_stomach, swelled_lymph_nodes, malaise, blurred_and_distorted_vision, phlegm, throat_irritation, redness_of_eyes, sinus_pressure, runny_nose, congestion, chest_pain, weakness_in_limbs, fast_heart_rate, pain_during_bowel_movements, pain_in_anal_region, bloody_stool, irritation_in_anus, neck_pain, dizziness, cramps, bruising, obesity, swollen_legs, swollen_blood_vessels, puffy_face_and_eyes, enlarged_thyroid, brittle_nails, swollen_extremeties, excessive_hunger, extra_marital_contacts, drying_and_tingling_lips, slurred_speech, knee_pain, hip_joint_pain, muscle_weakness, stiff_neck, swelling_joints, movement_stiffness, spinning_movements, loss_of_balance, unsteadiness, weakness_of_one_body_side, loss_of_smell, bladder_discomfort, foul_smell_of_urine, continuous_feel_of_urine, passage_of_gases, internal_itching, toxic_look_(typhos), depression, irritability, muscle_pain, altered_sensorium, red_spots_over_body, belly_pain, abnormal_menstruation, dischromic_patches, watering_from_eyes, increased_appetite, polyuria, family_history, mucoid_sputum, rusty_sputum]

For using 'Check Doctor's availability' and 'Feedback' features, you can use the follwoing diseases ( as the model is trained for the following 41 diseases)
[Fungal infection, Allergy, GERD, Chronic cholestasis, Drug Reaction, Peptic ulcer disease, AIDS, Diabetes, Gastroenteritis, Bronchial Asthma, Hypertension, Migraine, Cervical spondylosis, Paralysis (brain hemorrhage), Jaundice, Malaria, Chicken pox, Dengue, Typhoid, Hepatitis A, Hepatitis B, Hepatitis C, Hepatitis D, Hepatitis E, Alcoholic hepatitis, Tuberculosis, Common Cold, Pneumonia, Dimorphic hemorrhoids(piles), Heart attack, Varicose veins, Hypothyroidism, Hyperthyroidism, Hypoglycemia, Osteoarthritis, Arthritis, (vertigo) Paroxysmal Positional Vertigo, Acne, Urinary tract infection, Psoriasis, Impetigo]

Note that the doctors data is limited as it is trained on mock doctors data. Hence for every disease, you will find 3-4 doctors only. However, we can use as large database as possible and the application is capable of handlling it.

Example of Feedback feature: 
1) click on disease from the above list. For example I searched Migraine. It will show a few doctors who are the best for treating it. 
2) click on give feedback button. and a fedback form will generate at the bottom. After clicking on submit feedback, you can give feedback to other doctors as well. The feedback along with rating will get saved in feedback.csv in datasets folder.
3) the next time you oprn this feedback page, the doctors will be arranged in decreasing order of their ratings given by users.

Example of Check doctor's availability feature:
1) Click on Check doctor's availability option in navigator bar. 
2) Type a disease say Allergy. Enter a time slot say 12.00PM -1.00PM. 
3) you will find the doctors available at that time slot.

Moreover you can explore chatbot feature by asking any kind of health related doubts.