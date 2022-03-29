import phonenumbers
from phonenumbers import timezones,carrier,geocoder

phonenumber = phonenumbers.parse('+916309499488')
timezone = timezones.time_zones_for_number(phonenumber,'en')
carrier = carrier.name_for_number(phonenumber,'en')
region = geocoder.description_for_number(phonenumber,'en')

print(phonenumber)
print(timezone)
print(carrier)
print(region)

