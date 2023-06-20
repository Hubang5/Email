/**
 * sendMarketingEmail
 * 
 * Sends a marketing email to a given list of recipients.
 * 
 * @param {string[]} recipients - An array of email addresses to send the email to.
 * @param {string} subject - The subject of the email.
 * @param {string} message - The body of the email.
 */
function sendMarketingEmail(recipients, subject, message) {
    // Create a new email object
    let email = {
        to: recipients,
        subject: subject,
        body: message
    };
    
    // Send the email
    Email.send(email);
}
