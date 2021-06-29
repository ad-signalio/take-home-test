# Organisation Management App

We want you to create a new prototype application for managing a large number of organisations.

An organisation is composed of many teams, with each team having a number of contacts. Contacts can only be assigned to
a single team at any one time.

### Models/Entities:

Organisation Team Contact

### Fields/Columns along with the validations against them:

An organisation should have:

- name (required, 255 characters max, case insensitive, and unique)

A team should have:

- name (required, case insensitive and unique within an organisation)

A contact should have:

- first_name (required, 255 characters)
- middle_name (255 characters)
- last_name (required, 255 characters)
- email (required, unique and must validate as an email address)

Given the above, we want you to create a prototype using rails to be able to create and manage organisations along with
its teams and contacts.

## Acceptance criteria:

- [ ] Must be a basic rails app.
- [ ] Must have a page listing all organisations
- [ ] The organisations' list/table must include a column for name and columns for option/link to show and edit for each
  row/organisation.
- [ ] Organisation index must have a button/link to navigate to create a new organisation.
- [ ] Organisation new form must have an input box for name followed by a submit button which creates the organisation
  and navigates to the organisation index page.
- [ ] Organisation new form must have a cancel button that takes the user back to the organisation index page. This
  button must first give the user an alert confirmation saying, "Are you sure you want to quit? you will lose all your
  form data" before redirecting the user.
- [ ] Organisation edit form similar to the new form will have the same capabilities, but instead of creating a new
  organisation, it updates it and redirects to organisation show page.
- [ ] Organisation show page must include the name of the organisation and a list/table of all teams within that
  organisation sorted by team name.
- [ ] The list/table of teams must include a column for name, number of contacts in the team and columns for
  options/links to show and edit team.
- [ ] Organisation show must have a button/link to navigate to create a new team within that organisation.
- [ ] Team new form must have an input box for name followed by a submit button, creating the team.
- [ ] Team new form must have a cancel button that takes the user back to the organisation show page. This button must
  first give the user an alert confirmation saying, "Are you sure you want to quit? you will lose all your form data "
  before redirecting the user.
- [ ] team edit form similar to the new form will have the same capabilities, but instead of creating a new team, it
  updates it and navigates to the team show page.
- [ ] Team show page must include the name of the team and a list/table of all contacts within that team sorted by first
  name and last name.
- [ ] The list/table of contacts must include a column for full name, email and columns for options/links to show and
  edit a contact.
- [ ] Team show must have a button/link to navigate to create new contact within that team.
- [ ] Contact new form must have an input box for the first name, last name, and email followed by a submit button which
  creates the team.
- [ ] Contact new form must have a cancel button which takes the user back to the team show page - this button must
  first give the user an alert confirmation saying, "Are you sure you want to quit? you will lose all your form data"
  before redirecting the user.
- [ ] Contact edit form similar to the new form will have the same capabilities, but instead of creating a new contact, it
  updates it and navigates to the team show page.
- [ ] Contact show page must include the full name of the contact and email.
- [ ] All pages must be reasonably designed (we love bootstrap but feel free to use any CSS framework you're comfortable
  with or go vanilla CSS) - imagine it's a website you will present to a client.
- [ ] All forms must consider any validations on the model/entity and display them appropriately.
- [ ] We expect tests for all of this. (We'd love to see feature tests on top of any unit tests).

### Bonus

- [ ] On the contact show page, there must be a link next to the email, which, if clicked, copies the email into the clipboard so a user can paste it into another app.
- [ ] Improve the user experience by adding a global navigation bar and identifying where we could add any buttons or
  links (such as back buttons or breadcrumbs) to help the user navigate the application.
- [ ] Add a Docker and compose file that allows a user to run the application inside a containerised environment
- [ ] Add a Helm file that would allow the application to be run on a Kubernetes cluster.
