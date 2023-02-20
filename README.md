# SQL
Easy Tasks

1)select first_name ,last_name,gender from patients where gender like 'm%'
2)select first_name,last_name from patients where allergies is null
3)select first_name from patients where first_name like 'c%'
4)update patients set allergies = 'NKA' where allergies is null
5)select concat (first_name,' ' ,last_name) as full_name from patients
6)select first_name,last_name,province_name from patients join province_names on province_names.province_id=patients.province_id
7)select count (patient_id)from patients where year(birth_date)=2010
8)select first_name,last_name,max(height) from patients
9)select * from patients where patient_id in  ('1','45','534','879','1000')
10)select count(admission_date) from admissions
11)select * from admissions where admission_date=discharge_date
12)select patient_id,count(admission_date) from admissions where patient_id= 579
13)select distinct(city) from patients where province_id='NS'
14)select first_name,last_name,birth_date from patients where height>160 and weight>70
15)select first_name,last_name,allergies from patients where city = 'Hamilton' and allergies is not null
16)select distinct city from patients where city like 'a%'or city like 'e%'or city like'i%'or city like 'o%'or city like 'u%' order by city asc;
