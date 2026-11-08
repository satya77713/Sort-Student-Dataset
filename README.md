#  Sort Student Dataset using Pandas

## Overview
This project is part of the Veda Technology AI & ML Internship.

The objective of this task is to sort a student dataset using Python and Pandas. Different numerical and categorical columns are sorted in ascending and descending order to understand how sorting helps organize and analyze data.

## Objective
To understand how to sort a Pandas DataFrame using the `sort_values()` method.

## Dataset Information
- **Dataset:** Student Dataset
- **File:** `student_data.csv`
- **Format:** CSV
- **Notebook:** `Sort_Student_Dataset.ipynb`

## Tools & Technologies
- Python
- Pandas
- Google Colab
- Jupyter Notebook

## Sorting Operations Performed

### 1. Sort Age in Ascending Order
Sorts students from the youngest to the oldest.

```python
ascending_sort = df.sort_values(
    by='age',
    ascending=True
)
```

### 2. Sort Age in Descending Order
Sorts students from the oldest to the youngest.

```python
descending_sort = df.sort_values(
    by='age',
    ascending=False
)
```

### 3. Sort by School
Sorts student records by school name in ascending order.

```python
school_sort = df.sort_values(
    by='school',
    ascending=True
)
```

### 4. Sort by Study Time
Sorts students by study time in descending order.

```python
study_sort = df.sort_values(
    by='studytime',
    ascending=False
)
```

### 5. Sort by Absences
Sorts student records by absences in ascending order.

```python
absence_sort = df.sort_values(
    by='absences',
    ascending=True
)
```

### 6. Sort by Final Grade (G3)
Sorts students by their final grade in descending order and resets the DataFrame index.

```python
grade_descending = df.sort_values(
    by='G3',
    ascending=False
)

reset_sort = grade_descending.reset_index(drop=True)
```

## Key Concepts Learned
- Loading CSV files using Pandas.
- Understanding DataFrame structure.
- Sorting numerical columns.
- Sorting categorical columns.
- Ascending and descending sorting.
- Using `sort_values()`.
- Resetting the DataFrame index using `reset_index()`.

## Project Structure

```text
Sort-Student-Dataset/
│
├── Sort_Student_Dataset.ipynb
├── student_data.csv
└── README.md
```

## How to Run
1. Download or clone this repository.
2. Open `Sort_Student_Dataset.ipynb` in Google Colab.
3. Upload the `student_data.csv` dataset to Colab.
4. Ensure the dataset path in the notebook is correct.
5. Run all code cells.
6. Observe the sorted student records.

## Learning Outcome
Successfully learned how to organize student records using Pandas sorting techniques. Practiced sorting numerical and categorical columns in ascending and descending order.

## Internship Details
- **Organization:** Veda Technology
- **Track:** AI & ML Internship
- **Task:** 20 – Sort Dataset

## Conclusion
This task improved my understanding of Pandas DataFrame sorting and demonstrated how sorting techniques can help organize and analyze student data efficiently.
