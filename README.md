# Daptin default market

This git repository contains schemas for a variety of applications which you can install in [Daptin](https://dapt.in). This market is present by default in a new instance. You can create your own repo and use it as a market among your users.

## Packages

Packages are smaller set of APIs you can pick and selectively install in Daptin. You can install these at any time after you have setup Daptin. Packages can define one or more of the following:

- Entities
  - Name: this defines the endpoint path
  - Columns/Fields
  - Indexes
  - Constraints
  - Validations
- Relations
  - among different entities
- Actions
  - Name: this defines the endpoint path
  - In fields: initial set of values/data required to invoke the user
  - Outcomes: set of invokations which take place chained one after the other
- State machines
  - Name: this defines the endpoint path
  - Initial event
  - States and events
- Exchanges
  - Syncing data with external sources
  - Google sheet endpoint 

## List of packages

| Schema                                                            | Entities                                  | Actions                                                           | State machines  | Description                                                                                |
| ----------------------------------------------------------------- | ----------------------------------------- | ----------------------------------------------------------------- | --------------- | ------------------------------------------------------------------------------------------ |
| [Blog](/blog)                                                     | blog, post, comment                       | Leave a comment, Create new post                                  | publish_status  | A single-user/multi-user blogging platform                                                 |
| [Contruction Project Management](/contruction-project-management) | construction                              | -                                                                 | -               | A basic entity designing demo                                                              |
| [Faq](/faq)                                                       | faq, merchant                             | -                                                                 | -               | Frequently answered questions platform                                                     |
| [Pay Via Paypal](/pay-via-paypal)                                 | -                                         | mark_as_complete_by_paypal, buy_package                           | -               | Integrate "Pay via Paypal" to any entity                                                   |
| [Store](/store)                                                   | inventory, sale                           | new_purchase, return item                                         | -               | A demonstrative schema showing how to use scripting in actions effectively                 |
| [Style](/style)                                                   | style, orders, vendors, cost, style_file  | new_order, sync with google sheet                                 | light_states    | A multi user designer cloth manufacturing management system                                |
| [Task List](/todolist)                                            | todo, tags, projects                      | new_task, mark_as_completed, new_project, new_data_exchange       | task_status     | Multi-user todo and task management platform with tags and projects                        |
| [Transactions and Payments](/transactions-and-payments)           | sale, payment                             | -                                                                 | -               | Requirement for the "Pay-via-Paypal" integration to maintain sales and payment information |

## How to install

- Goto *Dashboard*
- Goto *Market places*
- Find "Default market" in the list
- Click "Expand" to go to since marketplace item
- In actions, click "Install a package"
- Enter the "Name of the folder" of the package you want to install
- Submit, Daptin will restart to apply changes and expose new endpoints

### New to Daptin ?

[Find out more here](https://dapt.in)

## Package structure

Each folder can have the following files:

- JSON: schema files defining entities, actions and others parts
- CSV: to import as a data dump, if referenced by one of the JSON "imports"
- XLS: to import as a data dump, if referenced by one of the JSON "imports"