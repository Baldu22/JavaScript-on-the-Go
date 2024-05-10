# JavaScript-on-the-Go
// Function to check user role and password validity
function checkUserRoleAndPwd(role, password) {
    // Check user role
    if (role === "Department Head") {
        switch (password) {
            case "SiEsD3ptH34d":
                console.log("Welcome, Department Head!");
                break;
            default:
                console.log("Invalid password for Department Head.");
                break;
        }
    } else if (role === "Faculty") {
        switch (password) {
            case "SiEsF4cu1ty":
                console.log("Welcome, Faculty!");
                break;
            default:
                console.log("Invalid password for Faculty.");
                break;
        }
    } else if (role === "Student Officer") {
        switch (password) {
            case "#CCSOAko":
                console.log("Welcome, Student Officer!");
                break;
            default:
                console.log("Invalid password for Student Officer.");
                break;
        }
    } else if (role === "Student") {
        switch (password) {
            case "3SapatNa!":
                console.log("Welcome, Student!");
                break;
            default:
                console.log("Invalid password for Student.");
                break;
        }
    } else {
        console.log("Invalid user role.");
    }
}

// Test cases
checkUserRoleAndPwd("Department Head", "SiEsD3ptH34d"); // Correct password
checkUserRoleAndPwd("Faculty", "WrongPassword");        // Incorrect password
checkUserRoleAndPwd("Student Officer", "#CCSOAko");     // Correct password
checkUserRoleAndPwd("Student", "WrongPassword");        // Incorrect password
checkUserRoleAndPwd("Admin", "Password123");            // Invalid user role
