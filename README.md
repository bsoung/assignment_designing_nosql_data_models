# assignment_designing_nosql_data_models
I'll have one data model hold the SQL please

Benny and Greg

Basics
1.

## User

* username: String
  * Must contain only word characters
* password: String
  * Must be at least 8 characters
* email: String
  * Must contain an @ symbol
* timestamp

## Profile

* user: UserSchema
* aboutMe: string
* birthday: date type
  * Must be of type Date
* gender: String
  * Must be one of options
* phone number: number
  * Must be 10 characters
* location {
  * City: String
  * State: string
  * Country string
  }
* preferences {
  * birthdayVisibility: boolean,
  * genderVisibility: boolean,
  * phoneVisibility: boolean,
  * locationVisibility: boolean,
}
* timestamp: type Date


Intermediate
1.

## Reservation
  * user: UserSchema
  * reservationID: string
  * restaurant: RestaurantSchema
  * guests: Array
  * reservationTime: Date
  * timestamp: Date

## User
  * name: string
  * password: string
  * email: string
  * favorites: Array
  * phoneNumber: Integer
  * friends: Array
  * timestamp: date

## Restaurant

  * name
  * tables: Array
  * location {
    * City: String
    * State: string
    * Country: string
    }
  * rating: Integer
  * price: Integer
  * reviews: Array
  * timestamp: Date


2.

## Student
	* name: String
	* password: String
	* email
	* address
  * timestamp: date

## Exam
	* student: StudentSchema
	* grade: Integer
  * timestamp: date

## Class
	* subject: String
	* examGrades: Array
		* An array of Exams
  * exam: ExamSchema
  * student: StudentSchema
  * timestamp: date


## Semester
	* term: Integer
	* classes: Array
		* An array of Classes
  * timestamp: date

Advanced:

1.

## Product
  * department: DepartmentSchema
  * SKU: string
  * price: Integer
  * name: string
  * description: string
  * parentCompany: string
  * stock: Integer
  * timestamp: date


## Department
  * revenue: Array
    * Quarterly or monthly or yearly revenues
  * inventory: Array
     * of ProductSchema instances
  * name: string
  * transactions: Array
    * of ReceiptSchema instances
  * timestamp: date

## Receipt
  * department: DepartmentSchema
  * product: ProductSchema
  * transactionID: string
  * timestamp: date
