# csv-python-

#importing csv module
import csv
#csv file names
fields =['names', 'branch']
#data rows of csv file
rows =[ ['Anshul', 'COE'],
        ['ritwik', 'coe']]
#name of csv file
filename ="university_record.csv"
#writing top csv file
with open(filename,"w") as csvfile:
    #creating a csv writer object
    csvwriter= csv.writer(csvfile)

    # wrting the fields
    csvwriter.writerow(fields)
    #writing the data rows
    csvwriter.writerows(rows)
    print(rows)
