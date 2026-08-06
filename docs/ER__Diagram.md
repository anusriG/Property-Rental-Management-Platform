+----------------------+
                           |        ADMIN         |
                           +----------------------+
                           | admin_id (PK)        |
                           | name                |
                           | email               |
                           | password            |
                           +----------+----------+
                                      |
                                      | Manages
                                      |
                                      v
+----------------------+     Owns     +-----------------------+
|        OWNER         |------------->|       PROPERTY        |
+----------------------+              +-----------------------+
| owner_id (PK)        |              | property_id (PK)      |
| name                 |              | owner_id (FK)         |
| email                |              | title                 |
| phone                |              | address               |
| password             |              | rent_amount           |
+----------+-----------+              | property_type         |
           |                          | availability_status  |
           |                          +-----------+-----------+
           |                                      |
           |                                      | Receives
           |                                      |
           |                                      v
           |                         +--------------------------+
           |                         |     RENTAL REQUEST       |
           |                         +--------------------------+
           |                         | request_id (PK)          |
           |                         | customer_id (FK)         |
           |                         | property_id (FK)         |
           |                         | request_date             |
           |                         | status                  |
           |                         +-----------+-------------+
           |                                     |
           |                                     | Approved
           |                                     |
           |                                     v
+----------------------+              +--------------------------+
|      CUSTOMER        |              |        BOOKING          |
+----------------------+              +--------------------------+
| customer_id (PK)     |              | booking_id (PK)         |
| name                 |              | property_id (FK)        |
| email                |              | customer_id (FK)        |
| phone                |              | booking_date            |
| password             |              | move_in_date            |
+----------------------+              | payment_status          |
                                      +--------------------------+
