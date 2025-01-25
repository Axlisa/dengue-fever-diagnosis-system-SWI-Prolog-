% Facts
symptom(fever, 'Do you have fever? (yes/no)').
symptom(headache, 'Do you have headache? (yes/no)').
symptom(joint_pain, 'Do you have joint pain? (yes/no)').
symptom(rash, 'Do you have rash? (yes/no)').

% Rules
has_symptom(Symptom) :-
    symptom(Symptom, Query),
    write(Query),
    read(Response),
    Response = yes.

has_dengue_fever :-
    has_symptom(fever),
    has_symptom(headache),
    has_symptom(joint_pain),
    has_symptom(rash).

% Diagnosis
diagnose_disease :-
    has_dengue_fever,
    write('Based on the symptoms, you may have dengue fever.').

diagnose_disease :-
    \+ has_dengue_fever,
    write('Based on the symptoms, it is unlikely that you have dengue fever.').
