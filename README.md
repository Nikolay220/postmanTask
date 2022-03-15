# postmanTask

Registration response:
{
    "user": {
        "username": "nikolay",
        "email": "nikolayshutikov@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyMzA1YmFlZmQyMTFjMjEwMGRiMmFjMyIsInVzZXJuYW1lIjoibmlrb2xheSIsImV4cCI6MTY1MjUyMDM2NiwiaWF0IjoxNjQ3MzM2MzY2fQ.DvlYoOAHcHhX_21wMIcp66ZPIx2RL2tK72CApSIYwSw"
    }
}

Login response:
{
    "user": {
        "username": "nikolay",
        "email": "nikolayshutikov@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyMzA1YmFlZmQyMTFjMjEwMGRiMmFjMyIsInVzZXJuYW1lIjoibmlrb2xheSIsImV4cCI6MTY1MjUyMDk5MSwiaWF0IjoxNjQ3MzM2OTkxfQ.Suu3HrevUOjzM81xzahtgiB7P8dvQJpFG9apNSrbREE"
    }
}

Get current user response:
{
    "errors": {
        "message": "No authorization token was found",
        "error": {
            "name": "UnauthorizedError",
            "message": "No authorization token was found",
            "code": "credentials_required",
            "status": 401,
            "inner": {
                "message": "No authorization token was found"
            }
        }
    }
}

After adding token as param like this:
https://kata.academy:8021/api/user?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyMzA1YmFlZmQyMTFjMjEwMGRiMmFjMyIsInVzZXJuYW1lIjoibmlrb2xheSIsImV4cCI6MTY1MjUyMDk5MSwiaWF0IjoxNjQ3MzM2OTkxfQ.Suu3HrevUOjzM81xzahtgiB7P8dvQJpFG9apNSrbREE
{
    "errors": {
        "message": "No authorization token was found",
        "error": {
            "name": "UnauthorizedError",
            "message": "No authorization token was found",
            "code": "credentials_required",
            "status": 401,
            "inner": {
                "message": "No authorization token was found"
            }
        }
    }
}