Paytm Labs Data Engineer Challenge
Read the instructions below, and complete all the challenges. Your submission must
include the code used to solve this challenge.
*Disclaimer
We know that this dataset is small and can fit into any modern laptop with 2GB of ram.
Before you decide to use Pandas (for good reasons), please use any modern distributed
ETL (spark, flink, beam, dask, etc; spark preferred) because we expect your solution
to scale to larger datasets (TB or more)!
The Challenge
The Data
The weather data is available in this repo under: /data/2019/ . Sometimes a weather
station will not take readings for every field, in those situations, the station
reports all 9's for that field (exact value for missing fields are provided in the
table below). Make sure to deal with the missing values correctly.
FIELD TYPE DESCRIPTION MISSING
STN--- Int
Station number (WMO/DATSAV3 number) for the
location.
WBAN Int
WBAN number where applicable--this is the
historical "Weather Bureau Air Force Navy" number
- with WBAN being the acronym
YEARMODA Int. The year, month and day. yyyyMMdd
TEMP Real
Mean temperature for the day in degrees Fahrenheit
to tenths
9999.9
DEWP Real
Mean dew point for the day in degrees Fahrenheit
to tenths
9999.9
SLP Real
Mean sea level pressure for the day in millibars
to tenths
9999.9
STP Real
Mean station pressure for the day in millibars to
tenths
9999.9
VISIB Real Mean visibility for the day in miles to tenths 999.9
WDSP Real Mean wind speed for the day in knots to tenths. 999.9
MXSPD Real
Maximum sustained wind speed reported for the day
in knots to tenths
999.9
GUST Real
Maximum wind gust reported for the day in knots to
tenths
999.9
MAX Real Maximum temperature reported during the day in
Fahrenheit to tenths--time of max temp report
9999.9
