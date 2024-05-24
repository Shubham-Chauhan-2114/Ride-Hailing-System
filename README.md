# Ride-Hailing-System
DBMS Project

1. Scenario / Mini World Description
& Business Model
1. Introduction:
Our project focuses on developing an Intra-city Ride-Hailing Management System, which aims to
streamline the process of booking and managing rides for both passengers and drivers. This system will
facilitate the booking, tracking, and payment processes associated with ride-hailing services.
2. Entities:
- Rider: A person who requests rides through the ride-hailing application.
- Driver: Individuals who provide transportation services to passengers using their vehicles.
- Vehicle: The cars or vehicles used by drivers to provide transportation services.
- Trip: Each individual trip requested by a passenger and completed by a driver.
- Payment: Transactions between passengers and drivers for completed rides.
- Shift: Shift in which a driver will operate.
3. Functionalities:
- Registration and Authentication: Users (riders and drivers) can register for an account on the platform
using their email addresses or phone numbers.
- Booking Rides: Passengers can request rides by specifying their pickup and drop-off locations. The
system assigns the nearest available driver to the request.
- Tracking Rides: Passengers can track the location of their assigned driver in real-time until the
completion of the ride using their trip’s tracking ID.
- Driver Allocation: The system efficiently assigns ride requests to available drivers based on proximity
and other factors.
- Payment Processing: Once a ride is completed, the system calculates the fare based on distance, time,
and other relevant factors (dynamic pricing, etc.). Payments are processed securely through the
platform.
- Rating: Both passengers and drivers can rate each other and provide rating based on their experience
during the ride. This helps maintain service quality and accountability.
4. Data Requirements:
- User Data: Including personal information such as names, contact details, and account credentials
including rider and driver information.
3
- Trip Data: Information about each trip, including pickup/drop-off locations, timestamps, distance
traveled, fare, etc..
- Vehicle Data: Details about drivers, including vehicle information, availability status, and ratings.
- Payment Data: Transaction records, including payment methods, amounts, and timestamps.
- Rating Data: Ratings provided by riders and drivers after completing a trip.
5. Domain Description:
❖ We assume a Cab-Hailing service where users are divided into following sub-categories :-
● The attributes common to driver and rider are user_id, name, password, mail_id, DOB,
phone_num, address, avg_rating.
● The attributes specific to the driver include license_num, cut, shift_id, vehicle_id and
current_loc.
● The cut attribute will accumulate the amount which the driver has to pay to the
company. The cut is calculated at completion of each trip and the driver has to pay that
amount at the end of month to the company.
● The administrator is responsible for banning/unbanning any user who has a very low
rating. The administrator also has full access to the database. The administrator has the
prefix ‘admin’ in user_id.
❖ The Vehicle has attributes like vehicle_id, plate_num, seating_cap, type, color, model, and
status.
❖ The Trip Entity has pickup_loc, drop_loc, start, end, fare, dist, trip_id, tracking_id, status,
driver_id, rider_id, rating and payment_id.
❖ The Shift entity consists of shift_id, start and end.
❖ The Payment entity has payment_id, trip_id, timestamp and payment_mode and user_id.

