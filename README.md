# assignment_designing_nosql_data_models
I'll have one data model hold the SQL please

Benny and Greg

Basics
1.

## User
* profile: ProfileSchema
* username: String
  * Must contain only word characters
* password: String
  * Must be at least 8 characters
* email: String
  * Must contain an @ symbol
* timestamp

## Profile
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
  * restaurant: RestaurantSchema
  * reservationID: String (unique)
  * guests: Array
  * reservationTime: Date
  * timestamp: Date

## User
  * name: String (unique)
  * password: String
  * email: String (unique)
  * favorites: Array
  * phoneNumber: Integer
  * friends: Array
  * timestamp: Date

## Restaurant
  * name: String (unique)
  * tables: Array
  * city: String
  * state: String
  * country: String
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
  * class: ClassSchema
  * student: StudentSchema
  * exam: ExamSchema
	* subject: String
  * timestamp: date

## Semester
  * class: ClassSchema
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
     * of Products
  * name: string
  * transactions: Array
    * of Receipts
  * timestamp: date

## Receipt
  * department: DepartmentSchema
  * product: ProductSchema
  * transactionID: string
  * timestamp: date

2.

## Feed
	* user: UserSchema
	

## User
	* firstName: String 
	* lastName: String
	* email: String
	* profilePicture: String
	* password: String
	* friends: Array
		* An array of Users
	* activities: Array
		* An array of Posts
	* interactions: Array
		* An array interaction objects

## Post (activity)
	* user: UserSchema
	* title: String
	* text: String
	* image: String
	* timestamp: Date







