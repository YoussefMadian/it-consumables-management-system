## Release Date Filter (Previous Month)

Release_x0020_Date ge '@{outputs('StartOfLastMonth')}'
and Release_x0020_Date le '@{outputs('EndOfLastMonth')}'
