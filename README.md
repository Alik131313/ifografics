# ifografics<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Инфографика: Экономика Впечатлений</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #111827;
            color: #f3f4f6;
        }
        .chart-container {
            position: relative;
            margin: auto;
            height: 40vh;
            width: 100%;
            max-width: 800px;
            max-height: 400px;
        }
        .kpi-card {
            background-color: #1f2937;
            border-left: 4px solid #F7941E;
        }
        .flow-arrow {
            font-size: 2rem;
            line-height: 1;
            color: #F7941E;
        }
    </style>
    <!-- 
    Infographic Plan:
    1.  Introduction: Title and hook with key stat about digital consumption.
    2.  Section: Russia's Global Strategy. Visualized as a 4-step process using HTML/CSS.
    3.  Section: Key Audience Trends. A bar chart comparing the 5 main trends.
    4.  Section: The Digital Ecosystem's Response. Highlighting micro-dramas with a line chart and audience preferences with a donut chart.
    5.  Section: The Future of Content. Using big number callouts for key emotional drivers and case study stats.
    6.  Section: Bridging Worlds (Classical Arts & Animation). Contrasting audience sizes with a donut chart and a process diagram for cultural packaging.
    7.  Conclusion: Final summarizing thoughts.
    Color Palette: "Energetic & Playful" (#00A9E0, #F7941E, #F15A29, #8CC63F, #662D91).
    Visualization Choices:
    -   Key Stats (92%, $8.4B): Goal: Inform. Method: Big styled text (HTML/CSS). Justification: Direct and impactful.
    -   Russia's Strategy: Goal: Organize. Method: HTML/CSS Flexbox diagram. Justification: Shows a process flow clearly without SVG.
    -   Audience Trends: Goal: Compare. Method: Chart.js Bar Chart. Justification: Compares magnitudes of different qualitative concepts.
    -   Micro-drama Growth: Goal: Change. Method: Chart.js Line Chart. Justification: Ideal for showing trends over time.
    -   Audience Preferences: Goal: Compare. Method: Chart.js Donut Chart. Justification: Shows composition of a whole.
    -   Classical vs. Animation: Goal: Compare/Inform. Method: Chart.js Donut Chart and HTML/CSS diagram. Justification: Contrasts audience size and illustrates a process.
    -   No Mermaid JS or SVG graphics were used in this output. All visuals are rendered using Chart.js on Canvas or structured with HTML/CSS.
    -->
</head>
<body class="antialiased">

    <div class="container mx-auto p-4 md:p-8">

        <header class="text-center mb-12">
            <h1 class="text-4xl md:text-6xl font-black text-white mb-4">Экономика Впечатлений</h1>
            <p class="text-xl md:text-2xl text-gray-300 max-w-3xl mx-auto">Как завоевать внимание аудитории в эпоху тотальной цифровизации</p>
        </header>

        <main class="space-y-16">

            <section id="hook" class="text-center">
                 <div class="kpi-card rounded-xl shadow-2xl p-8 max-w-4xl mx-auto">
                    <p class="text-2xl text-gray-300 mb-2">Ключевая метрика цифровой эпохи:</p>
                    <div class="text-7xl md:text-8xl font-black text-orange-400 my-4">92%</div>
                    <p class="text-2xl text-gray-300">детей и подростков проводят в интернете по 6-7 часов ежедневно. Борьба идет не за лояльность, а за каждую секунду внимания.</p>
                </div>
            </section>

            <section id="strategy">
                <h2 class="text-3xl font-bold text-center mb-8">Стратегический компас России: 4 вектора успеха</h2>
                <p class="text-lg text-gray-400 text-center max-w-3xl mx-auto mb-10">
                   В глобальной конкуренции за эмоции недостаточно просто создавать контент. Эксперты выделяют комплексный подход, который позволяет не только быть услышанным, но и формировать культурную повестку.
                </p>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 text-center">
                    <div class="bg-gray-800 p-6 rounded-lg shadow-lg flex flex-col items-center">
                        <div class="text-5xl mb-4">🎭</div>
                        <h3 class="text-xl font-bold mb-2">Аутентичность</h3>
                        <p class="text-gray-400">Транслировать исконные ценности, не подражая, но и не замыкаясь в себе.</p>
                    </div>
                    <div class="bg-gray-800 p-6 rounded-lg shadow-lg flex flex-col items-center">
                         <div class="text-5xl mb-4">📱</div>
                        <h3 class="text-xl font-bold mb-2">Актуальные форматы</h3>
                        <p class="text-gray-400">Говорить с "поколением Альфа" на языке коротких видео, стримов и интерактивного контента.</p>
                    </div>
                    <div class="bg-gray-800 p-6 rounded-lg shadow-lg flex flex-col items-center">
                        <div class="text-5xl mb-4">📢</div>
                        <h3 class="text-xl font-bold mb-2">Маркетинг и продвижение</h3>
                        <p class="text-gray-400">Упаковать и донести продукт до целевой аудитории, используя все каналы.</p>
                    </div>
                    <div class="bg-gray-800 p-6 rounded-lg shadow-lg flex flex-col items-center">
                        <div class="text-5xl mb-4">🤝</div>
                        <h3 class="text-xl font-bold mb-2">Международное партнерство</h3>
                        <p class="text-gray-400">Создавать совместные проекты для кросс-культурного обмена и знакомства с Россией.</p>
                    </div>
                </div>
            </section>
            
            <section id="trends">
                <h2 class="text-3xl font-bold text-center mb-8">Пульс аудитории: 5 ключевых запросов</h2>
                <p class="text-lg text-gray-400 text-center max-w-3xl mx-auto mb-10">Социальное проектирование эмоций начинается с понимания глубинных потребностей людей. Аналитики ВЦИОМ выделяют пять главных трендов, формирующих потребительские запросы на впечатления.</p>
                <div class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <div class="chart-container">
                        <canvas id="trendsChart"></canvas>
                    </div>
                </div>
            </section>

            <section id="ecosystems">
                <h2 class="text-3xl font-bold text-center mb-10">Ответ цифровых экосистем: адаптация и новые ниши</h2>
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                    <div class="bg-gray-800 p-6 rounded-lg shadow-lg">
                        <h3 class="text-2xl font-bold mb-4">Феномен микродрам: новый стандарт сторителлинга</h3>
                        <p class="text-gray-400 mb-4">На стыке классической драматургии и клипового мышления рождается новый формат. Микродрамы — это полноценные истории с завязкой и кульминацией, умещенные в 1-2 минуты. Это мост к новому поколению зрителей.</p>
                         <div class="kpi-card rounded-lg p-4 text-center my-4">
                            <p class="text-sm text-gray-300">Объем мирового рынка микродрам</p>
                            <div class="text-4xl font-black text-orange-400">$8.4 млрд</div>
                            <p class="text-sm text-gray-300">с прогнозом удвоения в ближайшие 3 года</p>
                        </div>
                        <div class="chart-container h-64 max-h-64">
                            <canvas id="microDramaChart"></canvas>
                        </div>
                    </div>
                    <div class="bg-gray-800 p-6 rounded-lg shadow-lg">
                        <h3 class="text-2xl font-bold mb-4">Предпочтения аудитории по поколениям</h3>
                        <p class="text-gray-400 mb-4">Потребление контента сильно отличается в зависимости от возраста. Понимание этих различий — ключ к персонализированным рекомендациям и удержанию внимания.</p>
                        <ul class="list-disc list-inside text-gray-300 space-y-2 mb-6">
                            <li><b>Зумеры:</b> предпочитают короткий контент, часто смотрят в ускоренном режиме (x2).</li>
                            <li><b>Миллениалы:</b> ищут лайфстайл-контент и сериалы.</li>
                            <li><b>Старшее поколение (45+):</b> выбирают знакомые форматы (новости, аналитика) и используют фоновый просмотр.</li>
                        </ul>
                        <div class="chart-container h-80 max-h-80">
                            <canvas id="audienceChart"></canvas>
                        </div>
                    </div>
                </div>
            </section>
            
            <section id="future-content">
                <h2 class="text-3xl font-bold text-center mb-8">Эмоции на продажу: что будет востребовано завтра?</h2>
                <p class="text-lg text-gray-400 text-center max-w-3xl mx-auto mb-10">В мире, перегруженном информацией, растет ценность контента, который дарит простые и сильные человеческие чувства. Продюсеры делают ставку на проекты, вызывающие глубокий эмоциональный отклик.</p>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                     <div class="bg-gray-800 p-8 rounded-lg shadow-lg text-center">
                        <div class="text-6xl font-black text-blue-400 mb-2">Искренность</div>
                        <p class="text-gray-400">Честный разговор с аудиторией, как в сериале "Слово пацана", цепляет все поколения и создает культурный феномен.</p>
                    </div>
                    <div class="bg-gray-800 p-8 rounded-lg shadow-lg text-center">
                        <div class="text-6xl font-black text-green-400 mb-2">Доброта</div>
                        <p class="text-gray-400">Люди устали от "хтони" и ищут светлые истории со счастливым концом, которые дарят надежду и веру в лучшее.</p>
                    </div>
                     <div class="bg-gray-800 p-8 rounded-lg shadow-lg text-center">
                        <div class="text-6xl font-black text-purple-400 mb-2">Семья</div>
                        <p class="text-gray-400">Традиционные ценности и семейные истории, как в шоу "Суперниндзя", находят отклик в сердце каждого зрителя.</p>
                    </div>
                </div>
            </section>
            
            <section id="bridging-worlds">
                <h2 class="text-3xl font-bold text-center mb-10">От элитарного искусства до глобальной анимации</h2>
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 items-center">
                    <div class="bg-gray-800 p-6 rounded-lg shadow-lg">
                        <h3 class="text-2xl font-bold mb-4">Классика: нишевость и глубина</h3>
                        <p class="text-gray-400 mb-4">Классическое искусство, будь то опера или балет, остается элитарным, привлекая узкий сегмент аудитории (3-5%). Его цель — не массовость, а катарсис, глубокое эмоциональное потрясение. Стриминговые сервисы помогают, но не заменяют живого опыта.</p>
                        <div class="chart-container h-80 max-h-80">
                            <canvas id="classicAudienceChart"></canvas>
                        </div>
                    </div>
                     <div class="bg-gray-800 p-6 rounded-lg shadow-lg">
                        <h3 class="text-2xl font-bold mb-4">Анимация: упаковка культурного кода</h3>
                        <p class="text-gray-400 mb-4">Для глобального успеха анимации недостаточно быть просто качественной. Нужно научиться упаковывать свою аутентичность и культурные коды в современные, понятные всему миру форматы, как это делает корейская анимация.</p>
                        <div class="mt-6 space-y-4">
                            <div class="text-center font-bold bg-gray-700 p-3 rounded-lg">НАЦИОНАЛЬНЫЙ КУЛЬТУРНЫЙ КОД</div>
                            <div class="text-center flow-arrow">▼</div>
                            <div class="flex justify-around items-center text-center">
                                <div class="bg-blue-900 p-3 rounded-lg w-1/3">Современный формат</div>
                                <div class="bg-green-900 p-3 rounded-lg w-1/3">Аутентичный сюжет</div>
                            </div>
                            <div class="text-center flow-arrow">▼</div>
                            <div class="text-center font-bold bg-orange-800 p-3 rounded-lg">ГЛОБАЛЬНЫЙ ПРОДУКТ</div>
                        </div>
                    </div>
                </div>
            </section>
        </main>
        
        <footer class="text-center mt-16 pt-8 border-t border-gray-700">
            <p class="text-gray-500">Инфографика на основе материалов панельной дискуссии об экономике впечатлений.</p>
        </footer>

    </div>

    <script>
    document.addEventListener('DOMContentLoaded', () => {
        
        const FONT_COLOR = '#f3f4f6';
        const GRID_COLOR = '#4b5563';
        const PALETTE = ['#00A9E0', '#F7941E', '#F15A29', '#8CC63F', '#662D91'];

        Chart.defaults.color = FONT_COLOR;
        Chart.defaults.borderColor = GRID_COLOR;

        function wrapLabels(label, maxWidth = 16) {
            if (typeof label !== 'string' || label.length <= maxWidth) {
                return label;
            }
            const words = label.split(' ');
            const lines = [];
            let currentLine = '';
            for (const word of words) {
                if ((currentLine + ' ' + word).trim().length > maxWidth && currentLine.length > 0) {
                    lines.push(currentLine);
                    currentLine = word;
                } else {
                    currentLine = (currentLine + ' ' + word).trim();
                }
            }
            if (currentLine.length > 0) {
                lines.push(currentLine);
            }
            return lines;
        }

        const tooltipTitleCallback = (tooltipItems) => {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
              return label.join(' ');
            }
            return label;
        };
        
        const defaultPlugins = {
            legend: {
                position: 'bottom',
                labels: {
                    font: { size: 14 }
                }
            },
            tooltip: {
                callbacks: {
                    title: tooltipTitleCallback
                },
                backgroundColor: '#1f2937',
                titleFont: { size: 16, weight: 'bold' },
                bodyFont: { size: 14 },
                padding: 12,
                cornerRadius: 8
            }
        };

        const trendsCtx = document.getElementById('trendsChart')?.getContext('2d');
        if (trendsCtx) {
            const labels = [
                'Тренд на антистресс (ASMR, уют)',
                'Ностальгия (ретро-дискурс)',
                'Дефицит времени (короткий контент)',
                'Дефицит живого общения (инфлюенсеры)',
                'Тренд на идентичность (поиск себя)'
            ];
            new Chart(trendsCtx, {
                type: 'bar',
                data: {
                    labels: labels.map(l => wrapLabels(l, 25)),
                    datasets: [{
                        label: 'Уровень запроса аудитории (условно)',
                        data: [85, 75, 95, 80, 70],
                        backgroundColor: PALETTE,
                        borderColor: PALETTE.map(c => c + 'AA'),
                        borderWidth: 1
                    }]
                },
                options: {
                    indexAxis: 'y',
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: {
                        x: {
                            beginAtZero: true,
                            grid: { color: GRID_COLOR }
                        },
                        y: {
                            grid: { display: false }
                        }
                    },
                    plugins: { ...defaultPlugins, legend: { display: false } }
                }
            });
        }

        const microDramaCtx = document.getElementById('microDramaChart')?.getContext('2d');
        if(microDramaCtx) {
            new Chart(microDramaCtx, {
                type: 'line',
                data: {
                    labels: ['Сейчас', 'Через 3 года'],
                    datasets: [{
                        label: 'Рост рынка микродрам ($ млрд)',
                        data: [8.4, 16.8],
                        fill: true,
                        backgroundColor: 'rgba(247, 148, 30, 0.2)',
                        borderColor: '#F7941E',
                        tension: 0.1,
                        pointBackgroundColor: '#F7941E',
                        pointRadius: 5
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: {
                        y: { beginAtZero: true, grid: { color: GRID_COLOR } },
                        x: { grid: { display: false } }
                    },
                    plugins: { ...defaultPlugins, legend: { display: false } }
                }
            });
        }

        const audienceCtx = document.getElementById('audienceChart')?.getContext('2d');
        if(audienceCtx) {
            new Chart(audienceCtx, {
                type: 'doughnut',
                data: {
                    labels: ['Короткие видео (Зумеры)', 'Сериалы и лайфстайл (Миллениалы)', 'ТВ-форматы (45+)', 'Пользовательский контент'],
                    datasets: [{
                        label: 'Предпочтения',
                        data: [40, 30, 20, 10],
                        backgroundColor: PALETTE,
                        hoverOffset: 4
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: defaultPlugins
                }
            });
        }
        
        const classicAudienceCtx = document.getElementById('classicAudienceChart')?.getContext('2d');
        if(classicAudienceCtx) {
            new Chart(classicAudienceCtx, {
                type: 'doughnut',
                data: {
                    labels: ['Аудитория классического искусства', 'Остальная аудитория'],
                    datasets: [{
                        data: [4, 96],
                        backgroundColor: ['#662D91', '#374151'],
                         hoverOffset: 4
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: defaultPlugins,
                    cutout: '60%'
                }
            });
        }
    });
    </script>
</body>
</html>
