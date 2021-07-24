# Angular JAM users list

### Homework

1. Brokedown `index.html` file into separate reusable components using techniques from the lesson and place them into the `components.module.ts` module.

2. Create a new Dashboard page using the command `ng g module pages/dashboard --routing` and include id into `app-routing.module.ts` with the following structure. Don't forget to import `SharedModule` into the `DashboardModule` to use your components.

```
{
    path: 'dashboard',
    loadChildren: () =>
      import('../pages/dashboard/dashboard.module').then(
        m => m.DashboardModule
      ),
  },
```
3. Implement Table component and render list of users form the `people.json` file using `*ngFor`