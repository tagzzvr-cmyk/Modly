
const moderators = [
  { name: "ExampleMod1", role: "Senior Moderator" },
  { name: "ExampleMod2", role: "Moderator" },
  { name: "ExampleMod3", role: "Junior Moderator" },
  { name: "ExampleMod4", role: "Support" }
];

const search = document.getElementById("search");
const results = document.getElementById("results");

function displayModerators(query = "") {
  results.innerHTML = "";

  const filtered = moderators.filter(mod =>
    mod.name.toLowerCase().includes(query.toLowerCase()) ||
    mod.role.toLowerCase().includes(query.toLowerCase())
  );

  if (filtered.length === 0) {
    results.textContent = "No moderators found.";
    return;
  }

  filtered.forEach(mod => {
    const card = document.createElement("div");
    card.className = "result";

    const name = document.createElement("h3");
    name.textContent = mod.name;

    const role = document.createElement("p");
    role.textContent = "Role: " + mod.role;

    card.append(name, role);
    results.appendChild(card);
  });
}

search.addEventListener("input", () => {
  displayModerators(search.value);
});

displayModerators();
