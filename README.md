# LocalRentalSystem
a local rental system based on GCP/Django/React/Mysql

Functional Dependencies:
  TenantID → (Name, Email, Phone)
  OwnerID → (Name, Email, Phone)
  PropertyID → (Address, City, ZIP, Type, Rent, Bedrooms, Rating, OwnerID)
  (TenantID, PropertyID) → InterestDate
  LeaseID → (TenantID, PropertyID, StartDate, EndDate)
  PaymentID → (LeaseID, PaymentAmount, PaymentDate)
  ReviewID → (PropertyID, TenantID, Rating, ReviewDate, Comments)
  RequestID → (PropertyID, ContractorID, RequestDate, Description)
  NotificationID → (UserID, Message, NotificationDate)
