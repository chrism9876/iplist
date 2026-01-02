Source https://www.gstatic.com/ipranges/goog.json

added github action to auto update list (manual trigger)

curl https://www.gstatic.com/ipranges/goog.json | grep ipv4Prefix| awk -F ': ' '{print $2}' | tr -d '"' > goog.txt
