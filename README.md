<h1>Help Ticket System by <a href="https://www.linkedin.com/in/majidalirahmati/" target="_blank" rel="noopener noreferrer">Majid Ali</a></h1>


#### Project Idea

1. User can create a new help ticket
2. Admin can reply on help ticket
3. Admin can reject or resolve the ticket
4. When admin update on the ticket user will get one notification via email that ticket status is updated
5. User can give ticket title and description
6. User can upload a document like pdf or image

#### Table Structure

1. Tickets 
    - title ( string ) {required}, 
    - description ( text ) {required},
    - status (open {default}, resolved, rejected),
    - attachment ( string ) {nullable},
    - user_id ( int ) {required} filled by laravel,
    - status_changed_by_id ( int ) {nulled}

2. Replies 
    - body ( test ) {required},
    - user_id ( int ) {required} filled by laravel,
    - ticket_id ( int ) {required} filled by laravel