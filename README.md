# Creditinfo

1. DB can be created by creditinfo.sql
2. Replace connection string accordingly to your enviroment.
3. data file path and name is currently hardcoded to .\CreditInfoCandidateExam\CreditInfoImporter\bin\Debug\netcoreapp3.1 and name as "Sample.xml"
4. 


// 20211215043907
// https://localhost:44395/api/credit/Search?NationalID=AAA1240024

{
  "message": "Customer with National ID AAA1240024 does NOT exist"
}


--------------------------------------------------

// 20211215043802
// https://localhost:44395/api/credit/Detail?NationalID=AA0000011

{
  "firstname": "Milena",
  "lastName": "Dvorakova",
  "dateOfBirth": "1956-10-26T00:00:00",
  "gender": "Female",
  "nationalId": "AA0000011",
  "customerCode": "IND03",
  "contractDatas": [
    {
      "contractCode": "CC001",
      "roleOfCustomer": "Guarantor",
      "phaseOfContract": "Open",
      "originalAmount": 1000,
      "installmentAmount": 100,
      "currentBalanceAmount": 900,
      "overdueBalanceAmount": 0,
      "originalCurrency": "CZK",
      "installmentCurrency": "CZK",
      "currentBalanceCurrency": "CZK",
      "overdueBalanceCurrency": "CZK",
      "dateOfLastPayment": "2019-05-04T00:00:00",
      "nextPaymentDate": "2019-06-04T00:00:00",
      "dateAccountOpened": "2019-04-04T00:00:00",
      "realEndDate": "2020-03-04T00:00:00"
    },
    {
      "contractCode": "CC003",
      "roleOfCustomer": "MainDebtor",
      "phaseOfContract": "Closed",
      "originalAmount": 5600,
      "installmentAmount": 60,
      "currentBalanceAmount": 430,
      "overdueBalanceAmount": 20,
      "originalCurrency": "USD",
      "installmentCurrency": "USD",
      "currentBalanceCurrency": "USD",
      "overdueBalanceCurrency": "USD",
      "dateOfLastPayment": "2019-07-27T00:00:00",
      "nextPaymentDate": "2019-08-27T00:00:00",
      "dateAccountOpened": "2019-05-09T00:00:00",
      "realEndDate": "2022-03-27T00:00:00"
    }
  ],
  "sumofOriginalAmount": 6600,
  "sumofOriginalAmountCurrency": "USD",
  "sumofInstallmentAmount": 160,
  "sumofInstallmenttCurrency": "USD",
  "maxofOverdueBalance": 20,
  "maxofOverdueBalanceCurrency": "USD"
}
