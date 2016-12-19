
def login():
    email=input("Enter your username:")
    passw=input("Enter your password:")

    if (email, passw) == ("admin", "admin12"):
        print("username and password matched")
        print("\nyou are login as a physician\n")

    else:
        print ("Invalid username,please try again")


def alogin():
    email=input("Enter your username:")
    passw=input("Enter your password:")

    if (email, passw) == ("admin12", "admin"):
        print("username and password matched")
        print("\nWelcome,you are a accountant\n")

    else:
        print ("Invalid username,please try again")




print ("WElCOME TO THE PRUDENT HEALTH CARE CENTER")

file = "dic.txt"


def register(patient_id, first_name, last_name, address, gender, contact, patient_age):
    fw = open('dic.txt', "a")
    fw.write("%1s%20s%20s%20s%20s%20s%20s\n" % (patient_id, first_name, last_name, address, gender, contact, patient_age))
    fw.close()




textfile = "payment.txt"
def cost(invoice_id, treatment_id, Bill_amount):
    fw = open('payment.txt', "w")
    fw.write("%1s%20s%15s\n" % (invoice_id, treatment_id, Bill_amount))
    fw.close()


def gone(patient_id, treatment_id, cash):
    fw = open('ripayment.txt', "a")
    fw.write("%1s%20s%20s\n" % (patient_id, treatment_id, cash))
    fw.close()



def receipt():
    print ("Receipt payment process")
    patient_id = input("enter your patient id:")
    treatment_id = input("enter treatmentid:")
    cash = input("enter total cash:")
    gone(patient_id, treatment_id, cash)





def payment():

    print ("welcome to payment process")
    print ("press enter to continue the payment process")
    invoice_id = input("please enter your invoice id:")
    print (invoice_id)
    Bill_amount = input(" Please enter bill amount:")
    print (Bill_amount)
    treatment_id =input(" Please enter treatment id:")
    print (treatment_id)
    cost(invoice_id, treatment_id, Bill_amount )
    print("Thank you")




def st():
    users = open("payment.txt", 'r')
    extract = input("Please input patient ID:")
    for each_line in users:
        (invoice_id, treatment_id, Bill_amount) = each_line.split()

    if (invoice_id == extract):
        print(invoice_id, treatment_id, Bill_amount)
    else:
        print ("error")


def registration():
    patient_id = input("Enter patient_id:")
    print (patient_id)
    first_name =input("Enter your first_name:")
    print (first_name)
    last_name = input("Enter your last name:")
    print (last_name)
    address = input("Enter your address:")
    print (address)
    gender = input("Enter your gender: ")
    print (gender)
    contact = input("Enter your contact number:")
    print (contact)
    patient_age = input("date of birth:")
    print (patient_age)
    register(patient_id, first_name, last_name, address, gender, contact, patient_age)
    print("THANK YOU!!!")
    print("\nUser created!\n")


file = "appointment.txt"



def writes(appointment_id, select_doctor, doctor_time, status):
    fw = open('appointment.txt', "a")
    fw.write("%1s%20s%20s%10s\n" % (appointment_id, select_doctor, doctor_time,  status))
    fw.close()



def appointment():
    print("Book an appointment")
    appointment_id=input("enter appointment id:")
    print (appointment_id)
    select_doctor = input("enter name of Doctor:")
    print (select_doctor)
    doctor_time= input("Select  appointment time")
    status = input("enter status:")
    print (status)
    writes(appointment_id, select_doctor, doctor_time, status)


def history(treatment_id, complaint, treatment):
    fw = open('treatment.txt', "a")
    fw.write("%1s%20s%20s\n" % (treatment_id, complaint, treatment))
    fw.close()


def treatment():
    print ("press enter to start a patient treatment plan")
    treatment_id = input("enter the treatement id:")
    print (treatment_id)
    complaint =input("enter the complaint of patient:")
    print (complaint)
    treatment =input(" write a treatment detail of a patient:")
    print (treatment)
    history(treatment_id, complaint, treatment)
    print ("patient treatment record have been saved")
    print ("Thank you for your treatment")



def users():
    print("Login Page")
    status = ""

while True:
    print("Are you \n1.Physician\n2.Accountant")
    status = input("User")

    if status =="1":
        email = input("Enter your username:")
        passw = input("Enter your password:")

        if (email, passw) == ("admin", "admin12"):
            print("username and password matched")
            print("\n welcome,you are physician\n")

        else:
            print ("Invalid username,please try again")
            continue



        while True:
            users=input("1.registration\n2.appointment\n3.treatment\n4.exist")
            if users=="1":
                registration()

            elif users=="2":
                appointment()


            elif users=="3":
                treatment()


            elif users == "4":
                exit()

            break

        else:
            print("wrong choice")

    elif status == "2":
        email = input("Enter your username:")
        passw = input("Enter your password:")

        if (email, passw) == ("admin12", "admin"):
            print("username and password matched")
            print("\nWelcome,you are a accountant\n")


        else:
            print ("Invalid username,please try again")
            continue



        while True:
            users = input("1.Invoicing\n2.Search patient\n3.Receipt payment\n4.Exist")

            if users == "1":
                payment()


            elif users =="2":

                st()

                print ("Search the  payment detail of the patient")

            elif users == "3":
                receipt()


            elif users == "4":
                print ("Quite")
                break


