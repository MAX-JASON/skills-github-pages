<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>廖啟梅意外險分析建議</title>
    <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h1, h2, h3 {
            color: #333;
        }
        .chart-container {
            margin-bottom: 40px;
        }
    </style>
</head>
<body>
    <h1>廖啟梅意外險分析建議</h1>

    <!-- 1. 新舊保單對比 -->
    <div class="chart-container">
        <h2>1. 新舊保單對比</h2>
        <div id="policyComparisonChart" style="width:100%;height:400px;"></div>
        <p>新保單的理賠額度更高，保障範圍更廣，能更好地應對意外風險。</p>
    </div>

    <!-- 2. 年長者意外風險趨勢 -->
    <div class="chart-container">
        <h2>2. 年長者意外風險趨勢</h2>
        <div id="riskByAgeChart" style="width:100%;height:400px;"></div>
        <p>60 歲以上族群的意外風險顯著上升，保障需求更高。</p>
    </div>

    <!-- 3. 未來醫療開銷預估 -->
    <div class="chart-container">
        <h2>3. 未來醫療開銷預估</h2>
        <div id="medicalCostChart" style="width:100%;height:400px;"></div>
        <p>根據統計，60 歲以上族群平均每年意外醫療開銷約為 $50,000 元，未來 20 年總開銷可能高達 $1,000,000 元。</p>
        <p><strong>小故事：</strong>張阿姨今年 65 歲，去年因意外跌倒導致骨折，醫療費用高達 $80,000 元。幸好她有完善的意外險，減輕了經濟負擔。</p>
    </div>

    <script>
        // 確保 DOM 元素加載完成後再執行
        document.addEventListener("DOMContentLoaded", function() {
            // 1. 新舊保單對比
            const policyComparisonData = [
                {
                    x: ['理賠額度', '保障項目', '保障年限'],
                    y: [20000, 1, 1], // 舊保單
                    type: 'bar',
                    name: '舊保單',
                    marker: { color: '#36A2EB' }
                },
                {
                    x: ['理賠額度', '保障項目', '保障年限'],
                    y: [500000, 4, 10], // 新保單
                    type: 'bar',
                    name: '新保單',
                    marker: { color: '#FF6384' }
                }
            ];
            const policyComparisonLayout = {
                title: '新舊保單對比',
                xaxis: { title: '項目' },
                yaxis: { title: '數值' },
                barmode: 'group'
            };
            Plotly.newPlot('policyComparisonChart', policyComparisonData, policyComparisonLayout);

            // 2. 年長者意外風險趨勢
            const riskByAgeData = [
                {
                    x: [40, 50, 60, 70, 80],
                    y: [10, 15, 25, 35, 50],
                    type: 'scatter',
                    mode: 'lines+markers',
                    name: '意外風險 (%)',
                    line: { color: '#FF6384' }
                }
            ];
            const riskByAgeLayout = {
                title: '年長者意外風險趨勢',
                xaxis: { title: '年齡' },
                yaxis: { title: '意外風險 (%)' }
            };
            Plotly.newPlot('riskByAgeChart', riskByAgeData, riskByAgeLayout);

            // 3. 未來醫療開銷預估
            const medicalCostData = [
                {
                    x: [60, 65, 70, 75, 80],
                    y: [50000, 60000, 70000, 80000, 90000],
                    type: 'bar',
                    name: '年醫療開銷',
                    marker: { color: '#9966FF' }
                }
            ];
            const medicalCostLayout = {
                title: '未來醫療開銷預估',
                xaxis: { title: '年齡' },
                yaxis: { title: '醫療開銷 (元)' }
            };
            Plotly.newPlot('medicalCostChart', medicalCostData, medicalCostLayout);
        });
    </script>
</body>
</html>
