# hermes-skills

Repo nguồn skill (tap) cho **Hermes Agent** — Công ty Á Châu (bluebedeli).

## Cách nối vào Hermes

```bash
hermes skills tap add bluebedeli/hermes-skills
```

Sau đó tìm skill trong repo:

```bash
hermes skills search <từ khóa> --source github
hermes skills install bluebedeli/hermes-skills/<skill>
```

## Skills trong repo

| Skill | Nhiệm vụ |
|-------|----------|
| `skills/find-skills` | Tự tìm & cài skill phù hợp cho từng công việc từ hệ sinh thái skills.sh: `npx skills find <từ khóa>` để khám phá, `npx skills add <owner/repo@skill>` để cài. Ưu tiên skill có nhiều lượt cài (1K+) từ nguồn chính thức (vercel-labs, anthropics). |

## Cấu trúc repo

```
hermes-skills/
├── README.md
└── skills/            ← thư mục mặc định Hermes tap đọc
    └── find-skills/
        └── SKILL.md
```

Thêm skill mới: tạo thư mục `skills/<ten-skill>/SKILL.md` (có frontmatter `name` + `description`), commit & push. Hermes tự nhận diện.
