## Start Of Last Month
startOfMonth(addToTime(utcNow(), -1, 'Month'))

## End Of Last Month
addSeconds(startOfMonth(utcNow()), -1)

## Stock Calculation
NewStock = CurrentStock - ReleasedQuantity
