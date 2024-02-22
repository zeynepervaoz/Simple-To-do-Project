# Simple-To-do-Project
cd examples/motoko/simple-to-do
dfx start --background
dfx deploy
dfx canister call simple_to_do addTodo '("Create a project")'
dfx canister call simple_to_do addTodo '("Build the project")'
dfx canister call simple_to_do addTodo '("Deploy the project")'
dfx canister call simple_to_do showTodos
("
___TO-DOs___
(1) Create a project
(2) Build the project
(3) Deploy the project")
dfx canister call simple_to_do completeTodo '(1)'
dfx canister call simple_to_do showTodos
("
___TO-DOs___
(1) Create a project ✔
(2) Build the project
(3) Deploy the project")
