# apiGo
Creating a mock api for learning Go


Test curls:

curl -vvv --data '{
    "Id": "2",
    "Title": "Newly Updated Post",
    "desc": "The description for my new post",
    "content": "my articles content"
}' -X PATCH 'http://localhost:10000/article'

 curl -vvv -X POST -m 10 -H "Expect:" -H "x-openrtb-version:2.2" -H "Content-Type:application/json" -d '{
    "Id": "3",
    "Title": "Newly Created Post",
    "desc": "The description for my new post",
    "content": "my articles content"
}' --url 'http://localhost:10000/article'

curl -vvv -X DELETE 'http://localhost:10000/article/2'
