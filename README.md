# Daptin default market

This git repository contains schemas for a variety of applications which you can install in [Daptin](https://dapt.in). This market is present by default in a new instance. You can create your own repo and use it as a market among your users.


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

