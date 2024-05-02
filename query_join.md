# Instructions

### Group by
1. Contare quanti iscritti ci sono stati ogni anno
    ```SQL
    SELECT YEAR(`enrolment_date`) AS 'enrollment_year', COUNT(id) AS 'enrolled_students' FROM `students` GROUP BY YEAR(`enrolment_date`);
    ```
    Result:
    ![alt text](image.png)

2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio
    ```SQL
    SELECT `office_address`, COUNT(id) AS 'teachers_in_this_building' FROM `teachers` GROUP BY `office_address`;
    ```
    Result:
    ![alt text](image-1.png)

3. Calcolare la media dei voti di ogni appello d'esame
4. Contare quanti corsi di laurea ci sono per ogni dipartimento

### Joins
1. Selezionare tutti gli studenti iscritti al Corso di Laurea in Economia
2. Selezionare tutti i Corsi di Laurea Magistrale del Dipartimento di Neuroscienze
3. Selezionare tutti i corsi in cui insegna Fulvio Amato (id=44)
4. Selezionare tutti gli studenti con i dati relativi al corso di laurea a cui sono iscritti e il relativo dipartimento, in ordine alfabetico per cognome e nome
5. Selezionare tutti i corsi di laurea con i relativi corsi e insegnanti
6. Selezionare tutti i docenti che insegnano nel Dipartimento di Matematica (54)
7. **BONUS**: Selezionare per ogni studente il numero di tentativi sostenuti per ogni esame, stampando anche il voto massimo. Successivamente, filtrare i tentativi con voto minimo 18.