#Codebook for Decapitated Animals Found in New York Parks

##Variable Descriptives

###animal
variable: ANIMAL, variable type: character field (variable length), variable label: the type of decapitated animal identified, note: in cases where more than one type of animal was identified, only the primary animal is listed.

###quantity
variable: QUANTITY, variable type: integer, variable label: the number of decapitated animals identified, note: in cases where the number of decapitated animals is ambiguous the smallest possible estimate is given. Note that though this variable may refer to parts of animals, it is given as an integer.

###body_part_found
variable: BODY_PART_FOUND, variable type: character field (variable length), variable label: the part of the decapitated animal identified.

###date_started
variable: DATE_STARTED, variable type: date, variable label: The date on which a report regarding the decapitated animal was first filed with the New York City Department of Parks and Recreation.

###date_closed
variable: DATE_CLOSED, variable type: date, variable label: The date on which the New York City Department of Parks and Recreation either resolved the issue regarding the decapitated animal, note: in cases where the New York City Department of Parks and Recreation did not resolve the issues regarding the decapitated animal, the date on which it did not resolve the issue regarding the decapitated animal is given.

###source
variable: SOURCE, variable type: categorical ("311-Call Center", "Department of Parks and Recreation"), variable label: The avenue by which the decapitated animal was originally identified.

###division
variable: DIVISION, variable type: categorical ("Borough Maintenance Operations Office - Queens", "Borough Maintenance Operations Office - Manhattan", "Borough Maintenance Operations Office - Bronx", "Borough Maintenance Operations Office - Brooklyn", "Borough Maintenance Operations Office - Staten Island", "Department of Parks and Recreation"), variable level: The division of the New York City Department of Parks and Recreation to which the decapitated animal was reported.

###form
variable: FORM, variable type: categorical ("DPR General Intake"), variable label: This is the form they use, note: There is only one form.

###status
variable: STATUS, variable type: categorical ("assigned", "closed"), variable label: This variable refers to whether The Department of Parks and Recreation is currently on the case.

###priority
variable: PRIORITY, variable type: ordinal, variable description: the level of priority, note: no known priority levels beyond normal exist.

###complaint_type
variable: COMPLAINT_TYPE, variable type: categorical ("animal in a park"), variable description: the niche occupied in the Department of Parks and Recreation's genre-classification of complaints, notes: full complaints classification schema is currently unknown.

###descriptor_1
variable: DESCRIPTOR_1, variable type: character field (variable length), variable description: a rich description of the substance of the complaint as reported.

###descriptor_2
variable: DESCRIPTOR_2, variable type: character field (variable length), variable description: a second rich description of the substance of the complaint as reported, note: words run dry.

###complaint_details
variable: COMPLAINT_DETAILS, variable type: character field (variable length), variable description: the details of the complaint, as heard by the Department of Parks and Recreation.

###location_type
variable: LOCATION_TYPE, variable type: categorical ("Park"), variable description: park, notes: park, park. park.

###park_or_facility
variable: PARK_OR_FACILITY, variable type: character (variable length), variable description: the specific park or facility in which the decapitated animal was reported to be, notes: the park could theoretically be a facility, fyi, but it is not; some cases not specified (code: "not specified").

###property_number
variable: property_number, variable type: array, variable description: some nonsense from the Parks Department, note: missing values of nonsense are blank.

###park_district
variable: PARK_DISTRICT, variable type: integer, variable description: the number of the park district in which the complaint was filed.

###additional_location_details
variable: additional_location_details, variable type: character field (variable length), variable description: specification of the location of decapitated animal within park, notes: values represented in all caps where originally rendered in purple crayon.

###council_district_number
variable: DISTRICT_NUMBER, variable type: integer, variable description: remaining number of months you have to live. jk. new york city council district in which the decapitated animal was identified.

###site_street_address
variable: SITE_STREET_ADDRESS, variable type: address, variable description: Street address of the New York City Department of Parks and Recreation site at which the decapitated animal was found.

###site_borough
variable: SITE_BOROUGH, variable type: categorical ("manhattan", "bronx", "brooklyn", "queens", "staten island"), variable description: The borough in which the site in which the identified decapitated animal is located.

###site_city_zip
variable: SITE_CITY_ZIP, variable type: array, variable description: The city and the zip code of the site in which the identified decapitated animal is located.

###lat
variable: LAT, variable type: numerical, variable description: latitude of decapitated animal.

###long
variable: LONG, variable type: numerical, variable description: latitude of decapitated animal.

###complaint_type_confirmed
variable: COMPLAINT_TYPE_CONFIRMED, variable type: categorical ("animal in a park"), variable description: please.

###descriptor_confirmed:
variable: DESCRIPTOR_CONFIRMED, variable type: character (variable length), variable description: i can't. note: all initial DPR descriptions perfectly capture facts on the ground.

###resolution_action_updated:
variable: RESOLUTION_ACTION_UPDATED, variable type: date, time. note: observations with values beginning with "4/1" for this variable should be interpreted with caution.

###resolution_description
variable: RESOLUTION_DESCRIPTION, variable type: character, (variable length), variable description: resolution of the decapitated animal.

###time_to_action
variable: TIME_TO_ACTION, variable type: categorical ("Closed: No Further Updates", "Past Due"), variable description: nothing to do with time to action.



##Appendices

Appendix 1:
Street addresses were used to identify the latitude and longitude of the park. In cases where street addresses were missing LAT and LONG were inferred according to a process of manual interpolation as follows: first, the park name alone was used; in cases where the park name was unavailable, the zip code in combination with the verbal description of the park were used in concert with visual inspection of a map.

Appendix 2:
Department of Parks and Recreation reports procured through FOILD program by Chen were transcribed by a freelancer named Hazel.
