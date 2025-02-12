## 1- Get the names of all cinema halls

```sql
SELECT name FROM cleaned_file;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/070971b6-e60c-41ed-ba23-928d3e3b9153" />


## 2- List all cinema halls with a rating of 4 

```sql
SELECT name FROM cleaned_file WHERE rating = 4;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/e98eaf1a-95e7-4735-a634-2832b37f3a64" />


## 3- Count how many cinema halls are there in total

```sql
SELECT COUNT(*) as total_cinema FROM cleaned_file;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/a283edc8-9cc7-4e71-80dc-dfc64c4ea7a3" />

## 4- Find cinema halls located in "Saudi Arabia"


```sql
SELECT name, location FROM cleaned_file WHERE location LIKE '%Saudi Arabia%';
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/cc82309b-f746-49ba-b5cd-facad2f9f555" />


## 5- Get the highest rating from the dataset

```sql
SELECT MAX(rating) as highest_rating FROM cleaned_file;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/97e1798f-511a-43b8-9390-f151e8c21ef5" />



## 6- List cinema halls with no reviews (review_count = 1)

```sql
SELECT name FROM cleaned_file WHERE review_count = 1;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/c4f6dad1-0fb8-4898-8287-8a8cd5c6b93d" />

## 7- Find the number of cinema halls for each rating

```sql
SELECT rating, COUNT(*) as count FROM cleaned_file GROUP BY rating;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/131aa6a2-a010-4001-b74e-6ac8691c203d" />


## 8- Retrieve cinema names and their genres

```sql
SELECT name, genre FROM cleaned_file;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/a189b4e7-a998-4a3b-bc90-e23bebb75cc1" />


## 9- Get cinema halls in "Al-kharj"

```sql
SELECT name FROM cleaned_file WHERE location LIKE '%Al-kharj%';

```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/496e41c0-c796-4afc-9dbc-5aa00c83d7d5" />


## 10- List cinema halls with a best comment available

```sql
SELECT name, best_comment FROM cleaned_file WHERE best_comment IS NOT NULL;
```
<img width="800" alt="image" src="https://github.com/user-attachments/assets/f848793b-52c0-4663-882f-9239821e1410" />
