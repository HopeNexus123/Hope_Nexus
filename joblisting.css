document.getElementById('submitJob').addEventListener('click', function () {
    const title = document.getElementById('jobTitle').value;
    const description = document.getElementById('jobDescription').value;
    const location = document.getElementById('location').value;
    const contact = document.getElementById('contact').value;

    if (title && description && location && contact) {
        // Create a new job entry
        const jobList = document.getElementById('jobItems');
        const jobItem = document.createElement('li');

        jobItem.innerHTML = `
            <strong>${title}</strong><br>
            <p>${description}</p>
            <em>Location: ${location}</em><br>
            <span>Contact: ${contact}</span>
        `;

        // Add the new job to the job list
        jobList.appendChild(jobItem);

        // Clear the form after submission
        document.getElementById('jobForm').reset();
    } else {
        alert('Please fill in all the fields!');
    }
});

// Search function
function searchJobs() {
    const query = document.getElementById('searchBar').value.toLowerCase();
    const jobs = document.getElementById('jobItems').getElementsByTagName('li');

    for (let i = 0; i < jobs.length; i++) {
        const jobText = jobs[i].textContent.toLowerCase();
        if (jobText.includes(query)) {
            jobs[i].style.display = '';
        } else {
            jobs[i].style.display = 'none';
        }
    }
}
