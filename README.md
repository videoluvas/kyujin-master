# vps-config

VPS (162.43.76.208) の設定ファイル管理リポジトリ。

## 構成

```
vps-config/
├── logrotate/
│   └── eizo-job        # ログローテーション設定
├── cron/
│   └── crontab         # cron設定
└── README.md
```

## デプロイ方法

### logrotate
```bash
cp logrotate/eizo-job /etc/logrotate.d/eizo-job
```

### cron
```bash
crontab cron/crontab
```

## 対象サービス

- `/var/www/eizo-job/app` — 映像求人PRO
- `/var/www/ai-job-pro/app` — AI映像求人PRO
