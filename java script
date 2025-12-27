// Lista på serier (data)
const seriesData = [
    { title: "Stranger Things", genre: "Sci-Fi", img: "https://picsum.photos/id/237/200/300" },
    { title: "The Bear", genre: "Drama", img: "https://picsum.photos/id/238/200/300" },
    { title: "Succession", genre: "Satir/Drama", img: "https://picsum.photos/id/239/200/300" },
    { title: "The Last of Us", genre: "Action/Äventyr", img: "https://picsum.photos/id/240/200/300" },
    { title: "The Crown", genre: "Historiskt Drama", img: "https://picsum.photos/id/241/200/300" }
];

const container = document.getElementById('series-container');

// Funktion för att visa serier
function displaySeries() {
    seriesData.forEach(serie => {
        const card = document.createElement('div');
        card.classList.add('series-card');
        
        card.innerHTML = `
            <img src="${serie.img}" alt="${serie.title}">
            <div class="series-info">
                <h3>${serie.title}</h3>
                <p>${serie.genre}</p>
            </div>
        `;
        
        container.appendChild(card);
    });
}

// Slumpa ett tips när man klickar på knappen
document.getElementById('cta-button').addEventListener('click', () => {
    const randomSerie = seriesData[Math.floor(Math.random() * seriesData.length)];
    alert(`Du borde kolla på: ${randomSerie.title}!`);
});

// Kör funktionen när sidan laddas
displaySeries();
