function stripGPS() {
    const gpsIndicator = document.getElementById('gps-indicator');
    // Simulate the washing process
    gpsIndicator.innerText = "⏳ Washing...";
    setTimeout(() => {
        gpsIndicator.innerText = "✅ GPS REMOVED";
        gpsIndicator.style.color = "#4caf50";
        updateAuditLog("Location Data Purged"); // Linking to your Audit Log
    }, 1500);
}

function stripID() {
    const idIndicator = document.getElementById('id-indicator');
    idIndicator.innerText = "⏳ Washing...";
    setTimeout(() => {
        idIndicator.innerText = "✅ ID REMOVED";
        idIndicator.style.color = "#4caf50";
        updateAuditLog("Device ID Purged");
    }, 1500);
}
