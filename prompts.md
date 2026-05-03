# Prompts for the Cursorist workshop

## A very naïve prompt

```
Build me a new landing page for a to-do application named Cursorist.
```

## A slightly better prompt

```
Build me a new landing page for a to-do application named Cursorist.

Use the attached image as the design to follow exactly.

Use Shadcn components where available.
```

## Cursor Rules

```
/create-rule

I want you to create a rule about the general application architecture to adhere to.

Aks me questions and come up with suggestions to decide what the rule file should contain.
```

```
Create a new page where I can see tasks I need to finish today under the path `/app/today`. Under the path `/app/inbox` I want to see a list of all tasks I need to complete.

I want a menu on the left of the screen to navigate between these views.

Just use a mock data structure for now.
```

```
On the @app/(tasks)/today/page.tsx route I would like an enhancement:
- Also show task which are not done yet and past their due date.

On the @app/(tasks)/inbox/page.tsx and @app/(tasks)/today/page.tsx routes I would also like to see a number of enhancements:
- When a task is past the due date the line with "Due: {date}" should be shown in red.
- Each item should have a checkbox to mark that task as done.
- Tasks with are not done and supposed to be done today should have their "Due: {date}" in green.
```

```
Update the Prisma schema to store the tasks in the database. Use the current mock data to seed the database. Make the @app/(tasks)/today/page.tsx and @app/(tasks)/inbox/page.tsx pages use the data from the database instead of the mock data they are using now.
```

```
npx prisma db seed
npx prisma studio
```

```
There is a problem with marking a task as done. The task disappears from the list but the database is never updated. When I refresh the page I see the original list of task again while I was expecting not to see the done task.
```

```
instead of a standard HTML checkbox I want to use the Shadcn Checkbox and Label components.

Make sure to use the best practices @Shadcn
```

```
I want to be able to add new tasks.

When enter the text date I want to be able to use a textual description to set the due date. For example:
- Add Playwright tests tomorrow
- Migrate to Supabase in two days
- Host the application on Vercel next week
- Add error logging next month

I also want to be able to just add the task title and select a due date manually using the Shadcn Date Picker component.
```

```
## Stitch Instructions

Get the images and code for the following Stitch project's screens:

## Project
Title: Todoist Redesign Dashboard
ID: 13452193057897107397

## Screens:
1. Todoist Redesign Dashboard
    ID: afd7370692174a90a08b7dd8b0f1ab80

Use a utility like `curl -L` to download the hosted URLs.
```

```
Apply this design to the /today and /inbox routes.
```
