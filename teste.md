```erDiagram LR
    USER ||--o{ POST : Referencia
    SIGNUP ||--o{ USER : Cria
    USER {
        string uid
        string email
        string display_name
        string photo_url
        datetime created_time
        string phone_number
        string bio
        string curso
        string linkedin
        string instagram
        integer seguidores
        integer seguindo
    }
    Comentarios ||--o{ POST : Referencia
    Comentarios ||--o{ USER : Referencia
    Comentarios {
        string CommentID
        datetime DateCreated
        string Content
        integer Likes
    }
    POST {
        string PostID
        datetime dateCreated
        string content
        Image Path photo
        Video Path video
        integer likes
    }
```
