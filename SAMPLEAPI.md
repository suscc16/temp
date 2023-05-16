Endpoint: /reward-points
HTTP Method: POST
Sample Request Body: 
{
  "transactions": [
    {
      "customer_id": "123",
      "date": "2023-04-15",
      "amount": 120.00
    },
    {
      "customer_id": "456",
      "date": "2023-04-20",
      "amount": 50.00
    },
    ...
  ]
}
Sample Response Body:
{
  "data": [
    {
      "customer_id": "123",
      "total_points": 270,
      "points_per_month": [
        {
          "month": "2023-04",
          "points": 90
        },
        {
          "month": "2023-05",
          "points": 90
        },
        {
          "month": "2023-06",
          "points": 90
        }
      ]
    },
    {
      "customer_id": "456",
      "total_points": 50,
      "points_per_month": [
        {
          "month": "2023-04",
          "points": 50
        },
        {
          "month": "2023-05",
          "points": 0
        },
        {
          "month": "2023-06",
          "points": 0
        }
      ]
    },
    ...
  ]
}
