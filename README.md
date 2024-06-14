## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

Original template can be found here: https://github.com/vercel/next-learn

### Changes
1. Fix [broken starter project](https://github.com/vercel/next-learn/issues/747)
2. Don't require a Vercel account - host the DB locally using Docker
    * https://github.com/vercel/storage/issues/123#issuecomment-2049389012
    * Noteworthy files:
        * [``./scripts/seed.js``](./scripts/seed.js)`
        * [``./app/lib/db.ts``](./app/lib/db.ts)
        * [``./app/lib/data.ts``](./app/lib/data.ts)
    * ⚠ When you develop after many reloads it might occur that the DB blocks creation of new clients with ``FATAL: sorry, too many clients already``.<br/>In this case: Simply restart the database
