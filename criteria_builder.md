# Sample Request

curl --location -g --request GET 'http://localhost:9000/api/v1/admin/user?page=1&size=20&filter[grant]=DIGITAL_FILE,d2f9c543-5ec7-4746-9967-93b8a66b0eb1&filter[first_name]=~~super&filter[email]=~~jonnyobell@gmail.com&filter[income_generated.1]=%3E=10&filter[sessions]=%3E=ONLINE,1&filter[user.subscription]=basic_membership&filter[state]=3566&filter[city]=1,2&filter[country]=240&filter[purchase]=basic_membership&filter[source]=1&filter[user.type]=1&filter[user.data.1]=company_industry,Computer%20Software&filter[user.data.2]=~~company_name,castlamp&filter[income_generated.2]=%3C=900&filter[created_at.1]=%3E=2020-01-01&filter[created_at.2]=%3C=2020-03-01' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2MTIxOTA5MzcsInVpZCI6MSwic2lkIjoiNjAxODE0ZDljNzc3NTguNjUxMDcxNTYiLCJleHAiOjE2MTIyNzczMzcsImlzcyI6ImxvY2FsaG9zdCJ9.w8gUR5hBy862FDkdedmUyHea-50PXSR9JZoXHeehS_E' \
--header 'Cookie: PHPSESSID=bosfcrtv3qd0f2979f56c3cibt'

- Notice how you can add a ".NUMBER" at the end to have the same mapper repeat:
    - user.data.1
    - user.data.2
    - user.data.3

- Input date format: yyyy-mm-dd


