# together
portfolio
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <title>포트폴리오 관리 시스템</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .table-header { background-color: #1e1b4b; color: white; }
        .bg-custom-yellow { background-color: #facc15; }
        .bg-custom-orange { background-color: #fb923c; }
    </style>
</head>
<body class="bg-gray-50 p-6">

    <div class="max-w-7xl mx-auto">
        <header class="flex justify-between items-center mb-6 border-b-2 border-gray-800 pb-2">
            <h1 class="text-2xl font-bold underline">포트폴리오 (대외비, 유포 시 법적 조치)</h1>
            <div id="auth-section">
                <button class="bg-blue-600 text-white px-4 py-2 rounded text-sm">로그인</button>
            </div>
        </header>

        <div class="overflow-x-auto shadow-2xl rounded-lg">
            <table class="w-full text-sm text-center border-collapse border border-gray-300">
                <thead>
                    <tr class="table-header">
                        <th class="p-3 border border-gray-300">구분(종목)</th>
                        <th class="p-3 border border-gray-300 bg-custom-yellow text-black">전시 비중</th>
                        <th class="p-3 border border-gray-300 bg-custom-orange text-red-700">추천가 (적정 매수)</th>
                        <th class="p-3 border border-gray-300 font-normal">예상 목표가</th>
                        <th class="p-3 border border-gray-300 font-normal">기대수익</th>
                        <th class="p-3 border border-gray-300 bg-custom-yellow text-black">현재가</th>
                        <th class="p-3 border border-gray-300 bg-custom-yellow text-red-600">수익률</th>
                        <th class="p-3 border border-gray-300 bg-custom-yellow text-black">비고 / 매매기록</th>
                    </tr>
                </thead>
                <tbody id="portfolio-body" class="bg-white">
                    <tr class="hover:bg-gray-50">
                        <td class="p-3 border font-bold bg-indigo-50">삼성전자</td>
                        <td class="p-3 border font-bold">2.0%</td>
                        <td class="p-3 border font-bold text-orange-600">95,000</td>
                        <td class="p-3 border bg-indigo-50 text-indigo-800">120,000</td>
                        <td class="p-3 border bg-indigo-50 text-indigo-800">26.3%</td>
                        <td class="p-3 border font-bold">78,500</td>
                        <td class="p-3 border font-bold text-blue-600">-17.3%</td>
                        <td class="p-3 border text-left text-xs text-gray-500">2024-03-20 신규 매수 진행</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="mt-8 p-6 bg-white border rounded-lg shadow-inner">
            <h2 class="font-bold mb-4 border-l-4 border-indigo-900 pl-2">내 종목 데이터 관리</h2>
            <div class="grid grid-cols-4 gap-4">
                <input type="text" placeholder="종목명" class="border p-2 rounded">
                <input type="number" placeholder="비중(%)" class="border p-2 rounded">
                <input type="number" placeholder="매수가" class="border p-2 rounded">
                <button class="bg-indigo-900 text-white rounded font-bold">데이터 업데이트</button>
            </div>
        </div>
    </div>

</body>
</html>
