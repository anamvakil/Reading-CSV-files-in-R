# Creating a data frame and reading CSV files in R

### 1. Installing and Loading the Package

 As we know the first step in RStudio is always loading and installing the packages that we need

![image](https://github.com/user-attachments/assets/dd0680cc-fd9f-430f-8732-21f85f49935f)

### 2. Creating dataframe

There are many ways to create a data frame in R, but one of the ways to do that is by creating individual data vectors and then combining them into a data frame using the `data.frame()` function.

![image](https://github.com/user-attachments/assets/8e2dd578-1270-4fbb-ab2b-dfedfbd1aa37)

Create a data frame named as "people" and populate it by using the above-mentioned vectors.

![image](https://github.com/user-attachments/assets/d87cc494-a23a-479b-a042-b267ab5cd4f4)

### 3. Inspecting the dataframe

Exploring some of the functions in R to summarize or preview the data as shown below.

![image](https://github.com/user-attachments/assets/b16e6443-78b5-4bb0-9e43-3fa6d4d512da)

![image](https://github.com/user-attachments/assets/504994e5-c953-4a62-871c-5721b368bc7a)

As we go further lets look at  `colnames()` function to get the column names from the table.

![image](https://github.com/user-attachments/assets/7f2efa85-6b61-49dd-bfeb-f0d9e179c8f0)

Similarly, we can use `mutate()` to add a new variable to your table.

![image](https://github.com/user-attachments/assets/62d4e3d2-0dac-4fc2-8816-e9ed136bcaf6)

The function helps us add a new variable to our dataframe that would capture each person's age in twenty years

# Reading CSV files in R

By using the `read_csv()` function we can import data from a .csv into a project folder called "hotel_bookings.csv" and save it as a data frame called `bookings_df` and performing the above listed functions on this csv file to explore that dataset further.

![image](https://github.com/user-attachments/assets/0d5e0da7-81e5-42be-b727-ccb548514912)

As we can see there are 119390 rows and 32 columns in this csv files. Functions can be of great use in such scenarios where the datasets that we need to look into are huge. We can use `head()` function to get the first 6 rows of the dataset in this csv file and get the insights of the table.

![image](https://github.com/user-attachments/assets/b8026385-2c04-4ace-a487-e51426153f86)

![image](https://github.com/user-attachments/assets/9e7ace48-7d8c-4647-85f5-8890bce9fca2)

the `str()` and function will provide summaries of each column in your data arranged horizontally

![image](https://github.com/user-attachments/assets/8e04d769-fd59-4af2-9f3b-354f87a41da9)

![image](https://github.com/user-attachments/assets/8ee8675c-3bef-49df-8a69-ca61fb142b71)

To find out what columns you have in your data frame, try running the the `colnames()` function in the code chunk below

![image](https://github.com/user-attachments/assets/cdf3977a-8b7b-460e-b4c6-92c5ca14b38f)

If you want to create another data frame using `bookings_df` that focuses on the average daily rate, which is referred to as `adr` in the data frame, and  `adults`

`new_df <- select(bookings_df, adr, adults)`

To create new variables in your data frame, you can use the `mutate()` function. This will make changes to the data frame, but not to the original data set you imported.

![image](https://github.com/user-attachments/assets/fd9a255c-bc85-4949-9751-901a3df5a067)

![image](https://github.com/user-attachments/assets/e691ffb5-e898-4ff5-8802-bf592e30e670)
