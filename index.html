<!doctype html>
<html lang="th" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ระบบบันทึกงานขนส่ง - แยกแถวถูกต้อง</title>
  <script src="https://cdn.tailwindcss.com/3.4.17"></script>
  <script src="https://cdn.jsdelivr.net/npm/lucide@0.263.0/dist/umd/lucide.min.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;600;700&amp;display=swap" rel="stylesheet">
  <style>
    * { font-family: 'Sarabun', sans-serif; }
    input[type="time"]::-calendar-picker-indicator { cursor: pointer; transform: scale(1.2); }
  </style>
 </head>
 <body class="h-full bg-slate-900 text-slate-100 overflow-auto">
  <div id="app" class="max-w-5xl mx-auto p-6">
   <h1 class="text-3xl font-bold text-amber-400 mb-6 text-center">ระบบบันทึกการส่งงานรถขนส่ง</h1>
   
   <div class="bg-slate-800 rounded-2xl p-4 mb-6 border border-slate-700 shadow-lg">
    <div class="grid sm:grid-cols-4 gap-3">
     <div>
      <label for="filter-view" class="block text-xs text-slate-400 mb-1">แสดงตามระยะเวลา</label> 
      <select id="filter-view" class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-white text-sm focus:outline-none"> 
       <option value="all">ทั้งหมด</option> 
       <option value="today">วันนี้</option> 
       <option value="week">สัปดาห์นี้</option> 
       <option value="month">เดือนนี้</option> 
      </select>
     </div>
     <div>
      <label for="filter-driver" class="block text-xs text-slate-400 mb-1">ผู้จัดส่ง</label> 
      <select id="filter-driver" class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-white text-sm focus:outline-none"> 
       <option value="">ทั้งหมด</option> 
      </select>
     </div>
     <div>
      <label for="filter-customer" class="block text-xs text-slate-400 mb-1">ลูกค้า</label> 
      <select id="filter-customer" class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-white text-sm focus:outline-none"> 
       <option value="">ทั้งหมด</option> 
      </select>
     </div>
     <div>
      <label class="block text-xs text-slate-400 mb-1">&nbsp;</label> 
      <button id="reset-filter" class="w-full bg-slate-600 hover:bg-slate-500 text-white text-sm px-3 py-2 rounded-lg transition-colors">รีเซ็ตตัวกรอง</button>
     </div>
    </div>
   </div>

   <div class="bg-slate-800 rounded-2xl p-6 mb-6 border border-slate-700 shadow-md">
    <h2 class="text-lg font-semibold text-amber-300 mb-4"><i data-lucide="plus-circle" class="inline w-5 h-5 mr-2 text-amber-400"></i>บันทึกเที่ยวส่งงานใหม่ (แยกแถวตรงตามหน้าชีต)</h2>
    <form id="delivery-form" class="grid sm:grid-cols-2 gap-4">
     <div class="sm:col-span-2">
      <div class="grid sm:grid-cols-3 gap-4 bg-slate-900/40 p-4 rounded-xl border border-slate-700/50">
       <div>
        <label for="trip-date" class="block text-sm text-slate-400 mb-1">วันที่ออกเดินทาง</label> 
        <input id="trip-date" type="date" required class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-white focus:outline-none">
       </div>
       <div>
        <label for="dep-time" class="block text-sm text-slate-400 mb-1">เวลาที่ออกรถ</label> 
        <input id="dep-time" type="time" required class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-amber-300 font-bold text-lg focus:outline-none">
       </div>
       <div>
        <label for="trip-id" class="block text-sm text-slate-400 mb-1">เลขที่เที่ยว (รันอัตโนมัติ)</label> 
        <input id="trip-id" type="text" readonly class="w-full bg-slate-700/70 border border-slate-600 rounded-lg px-3 py-2.5 text-amber-400 font-bold text-center" placeholder="ระบบกำลังสร้าง...">
       </div>
      </div>
     </div>

     <div>
      <label for="driver" class="block text-sm text-slate-400 mb-1">ชื่อผู้จัดส่ง</label> 
      <input id="driver" type="text" required class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-white focus:outline-none" placeholder="ระบุชื่อผู้ขับขี่">
     </div>
     <div>
      <label for="customer" class="block text-sm text-slate-400 mb-1">ลูกค้าปลายทาง</label> 
      <input id="customer" type="text" required class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-white focus:outline-none" placeholder="ชื่อบริษัทหรือร้านค้า">
     </div>

     <div class="sm:col-span-2">
      <label class="block text-sm font-semibold text-amber-300 mb-2">รายการใบแจ้งหนี้ในรอบรถนี้ (แยกแถวลงชีตอัตโนมัติ)</label>
      <div id="invoices-container" class="space-y-2 mb-3">
       <div class="invoice-item grid grid-cols-12 gap-2 items-center bg-slate-700/20 p-2 rounded-xl border border-slate-700">
        <div class="col-span-4">
         <select class="inv-prefix w-full bg-slate-700 border border-slate-600 rounded-lg px-2 py-2 text-white text-sm focus:outline-none"> 
          <option value="INVB-">INVB-</option> 
          <option value="INVN-">INVN-</option> 
          <option value="INMB-">INMB-</option> 
          <option value="INMN-">INMN-</option> 
         </select>
        </div>
        <div class="col-span-5">
         <input type="text" required class="inv-number w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-1.5 text-white text-sm focus:outline-none" placeholder="เลขที่เอกสาร">
        </div>
        <div class="col-span-2">
         <input type="text" value="2026" readonly class="inv-year w-full bg-slate-800 border border-slate-700 rounded-lg px-1 py-1.5 text-slate-500 text-sm text-center font-bold">
        </div>
        <div class="col-span-1 text-center">
         <button type="button" class="remove-invoice-btn text-red-400 hover:text-red-600 p-1"><i data-lucide="x-circle" class="w-5 h-5 mx-auto"></i></button>
        </div>
       </div>
      </div>
      <button type="button" id="add-invoice-btn" class="text-xs bg-slate-700 hover:bg-slate-600 text-amber-300 px-3 py-2 rounded-lg flex items-center gap-1"><i data-lucide="plus-circle" class="w-4 h-4"></i> เพิ่ม INV. ลงในเที่ยววิ่งนี้</button>
     </div>

     <div class="sm:col-span-2 mt-2">
      <button type="submit" id="submit-btn" class="w-full bg-amber-500 hover:bg-amber-600 text-slate-900 font-bold px-6 py-3 rounded-lg flex items-center justify-center gap-2 text-base"> 
       <i data-lucide="save" class="w-5 h-5"></i> บันทึกข้อมูลขึ้นชีตแยกแถว
      </button>
     </div>
    </form>
   </div>

   <div class="bg-slate-800 rounded-2xl p-6 border border-slate-700 shadow-md">
    <div class="flex justify-between items-center mb-4">
      <h2 class="text-lg font-semibold text-amber-300"><i data-lucide="calendar" class="inline w-5 h-5 mr-2 text-amber-400"></i>กระดานติดตามสถานะขนส่ง</h2>
      <button id="refresh-btn" class="p-2 bg-slate-700 hover:bg-slate-600 rounded-lg text-slate-300 flex items-center gap-1 text-xs"><i data-lucide="refresh-cw" class="w-3.5 h-3.5"></i> รีเฟรชข้อมูล</button>
    </div>
    <div id="records-list" class="space-y-4">
     <p id="empty-msg" class="text-slate-500 text-center py-4">กำลังโหลดข้อมูลจาก Google Sheet...</p>
    </div>
   </div>
  </div>

  <div id="modal" class="hidden fixed inset-0 bg-black/80 flex items-center justify-center z-50 p-4 backdrop-blur-sm">
   <div class="bg-slate-800 rounded-2xl p-6 w-full max-w-lg border border-slate-600 shadow-2xl">
    <div class="flex justify-between items-start mb-2">
      <h3 class="text-emerald-400 font-bold text-lg flex items-center gap-2"><i data-lucide="clock-4"></i> ลงบันทึกการกลับคลังรายใบงาน</h3>
      <span id="modal-trip-id" class="bg-slate-700 text-amber-400 font-bold text-xs px-2 py-1 rounded"></span>
    </div>
    <p id="modal-meta-display" class="text-xs text-slate-400 mb-4 border-b border-slate-700 pb-2"></p>
    
    <div class="mb-4">
      <label class="text-sm font-semibold text-slate-300 mb-2 block">ติ๊กเลือก INV ที่กลับเข้าคลัง (ไม่ติ๊ก = ต้องระบุสาเหตุ):</label>
      <div id="modal-invoice-list-container" class="space-y-2 bg-slate-900/50 p-3 rounded-xl max-h-60 overflow-y-auto border border-slate-700"></div>
    </div>

    <div class="mb-4">
      <label for="return-time" class="block text-xs text-slate-400 mb-1">เวลาที่รถกลับเข้าถึงคลัง (ใช้กับใบที่ติ๊กเลือก)</label> 
      <input id="return-time" type="time" required class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-white text-md font-bold focus:outline-none">
    </div>
    
    <div class="flex gap-3 mt-5">
     <button id="modal-save" class="bg-emerald-500 hover:bg-emerald-600 text-slate-900 font-bold px-4 py-2.5 rounded-lg flex-1 text-sm">ยืนยันลงบันทึก</button> 
     <button id="modal-cancel" class="bg-slate-600 hover:bg-slate-500 text-white px-4 py-2.5 rounded-lg flex-1 text-sm">ปิดหน้าต่าง</button>
    </div>
   </div>
  </div>

  <script>
  const GOOGLE_SCRIPT_URL = 'https://script.google.com/macros/s/AKfycbwJ_J-JGljo0Lyv0AGR9jF2wA4QR1Ig4BT_Dr0nPM__8z0KaJom7gAgBnSElyuaQuVHkQ/exec';

  let allRawRows = []; 
  let uniqueTrips = []; 
  let selectedTripData = null; 

  document.addEventListener('DOMContentLoaded', () => {
    const today = new Date();
    document.getElementById('trip-date').valueAsDate = today;
    const h = String(today.getHours()).padStart(2, '0');
    const m = String(today.getMinutes()).padStart(2, '0');
    document.getElementById('dep-time').value = `${h}:${m}`;
    fetchRecords();
  });

  function generateTripId(rawRows, targetDateString) {
    let dateObj = new Date();
    if(targetDateString) dateObj = new Date(targetDateString);
    const yy = String(dateObj.getFullYear()).slice(-2);
    const mm = String(dateObj.getMonth() + 1).padStart(2, '0');
    const dd = String(dateObj.getDate()).padStart(2, '0');
    const prefix = yy + mm + dd;
    const trackedIds = new Set(rawRows.map(r => String(r.trip_id)));
    const matchingIds = [...trackedIds].filter(id => id.startsWith(prefix));
    const seqs = matchingIds.map(id => parseInt(id.slice(-3)) || 0);
    const nextSeq = (Math.max(...seqs, 0) + 1).toString().padStart(3, '0');
    return prefix + nextSeq;
  }

  document.getElementById('trip-date').addEventListener('change', (e) => {
    document.getElementById('trip-id').value = generateTripId(allRawRows, e.target.value);
  });

  document.getElementById('add-invoice-btn').addEventListener('click', () => {
    const container = document.getElementById('invoices-container');
    const div = document.createElement('div');
    div.className = 'invoice-item grid grid-cols-12 gap-2 items-center bg-slate-700/20 p-2 rounded-xl border border-slate-700';
    div.innerHTML = `
        <div class="col-span-4">
         <select class="inv-prefix w-full bg-slate-700 border border-slate-600 rounded-lg px-2 py-2 text-white text-sm focus:outline-none"> 
          <option value="INVB-">INVB-</option> 
          <option value="INVN-">INVN-</option> 
          <option value="INMB-">INMB-</option> 
          <option value="INMN-">INMN-</option> 
         </select>
        </div>
        <div class="col-span-5">
         <input type="text" required class="inv-number w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-1.5 text-white text-sm focus:outline-none" placeholder="เลขที่เอกสาร">
        </div>
        <div class="col-span-2">
         <input type="text" value="2026" readonly class="inv-year w-full bg-slate-800 border border-slate-700 rounded-lg px-1 py-1.5 text-slate-500 text-sm text-center font-bold">
        </div>
        <div class="col-span-1 text-center">
         <button type="button" class="remove-invoice-btn text-red-400 hover:text-red-600 p-1"><i data-lucide="x-circle" class="w-5 h-5 mx-auto"></i></button>
        </div>
    `;
    container.appendChild(div);
    div.querySelector('.remove-invoice-btn').addEventListener('click', () => div.remove());
    lucide.createIcons();
  });

  async function fetchRecords() {
    const msgEl = document.getElementById('empty-msg');
    if(msgEl) msgEl.textContent = "กำลังโหลดข้อมูลจาก Google Sheet...";
    try {
      const response = await fetch(GOOGLE_SCRIPT_URL);
      allRawRows = await response.json();
      if(!Array.isArray(allRawRows)) allRawRows = [];
      document.getElementById('trip-id').value = generateTripId(allRawRows, document.getElementById('trip-date').value);
      processAndGroupData();
      buildFilterOptions();
      filterAndRenderHTML();
    } catch (err) {
      console.error(err);
      if(msgEl) msgEl.innerHTML = "⚠️ ดึงข้อมูลล้มเหลว โปรดตรวจสอบสัญญาณเครือข่าย";
    }
  }

  function processAndGroupData() {
    const map = {};
    allRawRows.forEach(row => {
      const tid = row.trip_id;
      if (!map[tid]) {
        map[tid] = {
          trip_id: tid,
          trip_date: row.trip_date,
          departure_time: row.departure_time,
          driver_name: row.driver_name,
          customer_name: row.customer_name,
          all_invoices: [] 
        };
      }
      if(row.invoice && !String(row.invoice).startsWith("[Ljava")) {
        map[tid].all_invoices.push({
          inv_code: row.invoice,
          return_time: row.return_time,
          note: row.note
        });
      }
    });
    uniqueTrips = Object.values(map);
  }

  function buildFilterOptions() {
    const drivers = new Set();
    const customers = new Set();
    uniqueTrips.forEach(t => {
      if(t.driver_name) drivers.add(t.driver_name);
      if(t.customer_name) customers.add(t.customer_name);
    });
    const dSel = document.getElementById('filter-driver');
    const cSel = document.getElementById('filter-customer');
    const dVal = dSel.value;
    const cVal = cSel.value;
    dSel.innerHTML = '<option value="">ทั้งหมด</option>' + [...drivers].sort().map(d => `<option value="${d}">${d}</option>`).join('');
    cSel.innerHTML = '<option value="">ทั้งหมด</option>' + [...customers].sort().map(c => `<option value="${c}">${c}</option>`).join('');
    dSel.value = dVal; cSel.value = cVal;
  }

  function filterAndRenderHTML() {
    const viewMode = document.getElementById('filter-view').value;
    const driverFilter = document.getElementById('filter-driver').value;
    const customerFilter = document.getElementById('filter-customer').value;
    const now = new Date();
    const todayStr = now.toISOString().split('T')[0];
    const currentDay = now.getDay();
    const startOfWeek = new Date(now);
    startOfWeek.setDate(now.getDate() - currentDay);
    startOfWeek.setHours(0,0,0,0);

    const filtered = uniqueTrips.filter(t => {
      if (driverFilter && t.driver_name !== driverFilter) return false;
      if (customerFilter && t.customer_name !== customerFilter) return false;
      if (!t.trip_date) return true;
      let tDateStr = t.trip_date.includes('T') ? t.trip_date.split('T')[0] : t.trip_date;
      if (t.trip_date.includes('/')) {
        const parts = t.trip_date.split('/');
        if(parts[2] && parts[2].length === 4) tDateStr = `${parts[2]}-${parts[1].padStart(2,'0')}-${parts[0].padStart(2,'0')}`;
      }
      const tDate = new Date(tDateStr + 'T00:00:00');
      if (viewMode === 'today') return tDateStr === todayStr;
      if (viewMode === 'week') return tDate >= startOfWeek;
      if (viewMode === 'month') return tDate.getFullYear() === now.getFullYear() && tDate.getMonth() === now.getMonth();
      return true;
    });
    renderRecordsContainer(filtered);
  }

  document.getElementById('filter-view').addEventListener('change', filterAndRenderHTML);
  document.getElementById('filter-driver').addEventListener('change', filterAndRenderHTML);
  document.getElementById('filter-customer').addEventListener('change', filterAndRenderHTML);
  document.getElementById('reset-filter').addEventListener('click', () => {
    document.getElementById('filter-view').value = 'all';
    document.getElementById('filter-driver').value = '';
    document.getElementById('filter-customer').value = '';
    filterAndRenderHTML();
  });
  document.getElementById('refresh-btn').addEventListener('click', fetchRecords);

  function renderRecordsContainer(trips) {
    const container = document.getElementById('records-list');
    container.innerHTML = '';
    if (trips.length === 0) {
      container.innerHTML = `<p class="text-slate-500 text-center py-6">ไม่มีข้อมูลการเดินรถ</p>`;
      return;
    }

    const groups = {};
    trips.forEach(t => {
      let d = 'ไม่มีกำหนดวันที่';
      if(t.trip_date) {
        d = t.trip_date.includes('T') ? t.trip_date.split('T')[0] : t.trip_date;
        if (t.trip_date.includes('/')) {
          const parts = t.trip_date.split('/');
          if(parts[2]) d = `${parts[2]}-${parts[1].padStart(2,'0')}-${parts[0].padStart(2,'0')}`;
        }
      }
      if(!groups[d]) groups[d] = [];
      groups[d].push(t);
    });

    Object.keys(groups).sort().reverse().forEach(dateStr => {
      const dateBlock = document.createElement('div');
      dateBlock.className = 'mb-3';
      let formatTitle = dateStr;
      try {
        const dObj = new Date(dateStr + 'T00:00:00');
        if(!isNaN(dObj)) formatTitle = new Intl.DateTimeFormat('th-TH', { year: 'numeric', month: 'long', day: 'numeric', weekday: 'long' }).format(dObj);
      } catch(e){}

      dateBlock.innerHTML = `<h3 class="text-amber-400 font-semibold text-xs mb-2 border-b border-slate-700 pb-1 mt-2"><i data-lucide="clock" class="inline w-3 h-3 mr-1"></i>${formatTitle}</h3>`;
      const subListBlock = document.createElement('div');
      subListBlock.className = 'space-y-2.5';

      groups[dateStr].forEach(trip => {
        const card = document.createElement('div');
        card.className = 'bg-slate-800/60 rounded-xl p-4 border border-slate-700/80 flex flex-col md:flex-row md:items-center md:justify-between gap-4 shadow-sm';
        
        let invBadgesHTML = '';
        let pendingCount = 0;
        
        trip.all_invoices.forEach(inv => {
          if (inv.return_time) {
            invBadgesHTML += `<span class="bg-emerald-500/10 text-emerald-400 text-xs border border-emerald-500/30 rounded-md px-2 py-0.5" title="กลับ: ${inv.return_time} [${inv.note || '-'}]">✓ ${inv.inv_code}</span>`;
          } else {
            pendingCount++;
            const noteText = inv.note ? ` (${inv.note})` : '';
            invBadgesHTML += `<span class="bg-slate-700 text-amber-300 text-xs border border-slate-600 rounded-md px-2 py-0.5">⏱ ${inv.inv_code}${noteText}</span>`;
          }
        });

        card.innerHTML = `
          <div class="flex-1 min-w-0">
            <div class="flex items-center gap-3 flex-wrap mb-2">
              <span class="bg-amber-400 text-slate-900 text-xs font-bold px-2 py-0.5 rounded shadow-sm">เที่ยวรถ: ${trip.trip_id}</span>
              <div class="flex flex-wrap gap-1">${invBadgesHTML}</div>
            </div>
            <div class="grid grid-cols-2 md:grid-cols-3 gap-y-1 gap-x-4 text-xs text-slate-400">
              <div>ผู้จัดส่ง: <strong class="text-slate-200">${trip.driver_name}</strong></div>
              <div>ลูกค้า: <strong class="text-slate-200">${trip.customer_name}</strong></div>
              <div>เวลาที่ออกรถ: <strong class="text-amber-300">${trip.departure_time} น.</strong></div>
            </div>
          </div>
          <div class="text-right flex items-center md:justify-end gap-2">
            ${pendingCount > 0 ? 
              `<button class="trigger-modal-btn bg-emerald-600 hover:bg-emerald-500 text-white text-xs font-bold px-4 py-2 rounded-lg flex items-center gap-1 shadow">
                <i data-lucide="check-square" class="w-4 h-4"></i> จัดการเวลากลับ/สาเหตุ
               </button>` : 
              `<span class="text-emerald-500 text-xs font-bold bg-emerald-500/10 border border-emerald-500/20 px-3 py-1.5 rounded-lg flex items-center gap-1"><i data-lucide="badge-check" class="w-4 h-4"></i> สำเร็จครบทุกรายการ</span>`
            }
          </div>
        `;

        const btn = card.querySelector('.trigger-modal-btn');
        if(btn) {
          btn.addEventListener('click', () => {
            selectedTripData = trip;
            openReturnModal(trip);
          });
        }
        subListBlock.appendChild(card);
      });
      dateBlock.appendChild(subListBlock);
      container.appendChild(dateBlock);
    });
    lucide.createIcons();
  }

  function openReturnModal(trip) {
    document.getElementById('modal-trip-id').textContent = `เที่ยวรถ: ${trip.trip_id}`;
    document.getElementById('modal-meta-display').textContent = `ผู้จัดส่ง: ${trip.driver_name} | ลูกค้า: ${trip.customer_name}`;
    
    const container = document.getElementById('modal-invoice-list-container');
    container.innerHTML = '';

    let hasItems = false;
    trip.all_invoices.forEach((inv) => {
      if(!inv.return_time) {
        hasItems = true;
        const rowDiv = document.createElement('div');
        rowDiv.className = 'bg-slate-800 p-3 rounded-xl border border-slate-700 space-y-2';
        rowDiv.innerHTML = `
          <div class="flex items-center justify-between">
            <label class="flex items-center gap-2 cursor-pointer font-semibold text-sm text-slate-100">
              <input type="checkbox" value="${inv.inv_code}" checked class="modal-inv-checkbox rounded text-emerald-500 w-4 h-4 bg-slate-700 border-slate-600">
              <span>${inv.inv_code}</span>
            </label>
            <span class="status-indicator-text text-xs text-emerald-400 font-medium">รถกลับเข้าคลัง</span>
          </div>
          <div class="reason-input-container hidden">
            <input type="text" class="modal-inv-reason w-full bg-slate-900 border border-red-500/50 rounded-lg px-3 py-1.5 text-xs text-white focus:outline-none" placeholder="* ระบุสาเหตุที่ใบงานนี้ยังไม่เข้าคลัง" value="${inv.note || ''}">
          </div>
        `;

        const cb = rowDiv.querySelector('.modal-inv-checkbox');
        const reasonContainer = rowDiv.querySelector('.reason-input-container');
        const statusText = rowDiv.querySelector('.status-indicator-text');
        const reasonInput = rowDiv.querySelector('.modal-inv-reason');

        cb.addEventListener('change', () => {
          if (cb.checked) {
            reasonContainer.classList.add('hidden');
            statusText.textContent = 'รถกลับเข้าคลัง';
            statusText.className = 'text-xs text-emerald-400 font-medium';
          } else {
            reasonContainer.classList.remove('hidden');
            statusText.textContent = 'ไม่เข้าคลัง (รอตรวจสอบ)';
            statusText.className = 'text-xs text-red-400 font-medium';
            reasonInput.focus();
          }
        });

        container.appendChild(rowDiv);
      }
    });

    if(!hasItems) {
      container.innerHTML = `<p class="text-xs text-slate-400 text-center py-2">ทุกใบงานในเที่ยวนี้ลงเวลากลับครบแล้ว</p>`;
    }

    const t = new Date();
    document.getElementById('return-time').value = `${String(t.getHours()).padStart(2, '0')}:${String(t.getMinutes()).padStart(2, '0')}`;
    document.getElementById('modal').classList.remove('hidden');
  }

  document.getElementById('modal-cancel').addEventListener('click', () => {
    document.getElementById('modal').classList.add('hidden');
    selectedTripData = null;
  });

  document.getElementById('modal-save').addEventListener('click', async () => {
    const returnTimeValue = document.getElementById('return-time').value;
    const itemRows = document.getElementById('modal-invoice-list-container').children;
    
    if (itemRows.length === 0) return;

    const invStatusMap = {};
    let isValidationError = false;

    for (let row of itemRows) {
      const cb = row.querySelector('.modal-inv-checkbox');
      if(!cb) continue;
      const reasonInput = row.querySelector('.modal-inv-reason');
      const invCode = cb.value;
      const isChecked = cb.checked;
      const reasonValue = reasonInput.value.trim();

      if (!isChecked && reasonValue === "") {
        alert(`กรุณาระบุสาเหตุของเลขที่ INV: ${invCode}`);
        reasonInput.focus();
        isValidationError = true;
        break;
      }

      invStatusMap[invCode] = { checked: isChecked, reason: reasonValue };
    }

    if (isValidationError) return;

    const btn = document.getElementById('modal-save');
    btn.disabled = true;
    btn.textContent = 'กำลังบันทึกสถานะ...';

    try {
      await fetch(GOOGLE_SCRIPT_URL, {
        method: 'POST',
        mode: 'no-cors',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({
          action: 'return_time',
          trip_id: selectedTripData.trip_id,
          return_time: returnTimeValue,
          inv_status_map: invStatusMap
        })
      });

      setTimeout(() => {
        document.getElementById('modal').classList.add('hidden');
        btn.disabled = false;
        btn.textContent = 'ยืนยันลงบันทึก';
        fetchRecords();
      }, 1200);

    } catch (err) {
      alert('เครือข่ายขัดข้อง');
      btn.disabled = false;
    }
  });

  document.getElementById('delivery-form').addEventListener('submit', async (e) => {
    e.preventDefault();
    const invItems = [];
    document.querySelectorAll('.invoice-item').forEach(el => {
      const pfx = el.querySelector('.inv-prefix').value;
      const num = el.querySelector('.inv-number').value.trim();
      const yr = el.querySelector('.inv-year').value;
      if (num) invItems.push(`${pfx}${num}-${yr}`);
    });

    if(invItems.length === 0) {
      alert('กรุณาระบุเลขที่ INV. ปลายทางครับ');
      return;
    }

    const subBtn = document.getElementById('submit-btn');
    subBtn.disabled = true;
    subBtn.textContent = 'ระบบกำลังแยกแถวบันทึก...';

    const payload = {
      action: 'new_trip',
      trip_id: document.getElementById('trip-id').value,
      trip_date: document.getElementById('trip-date').value,
      departure_time: document.getElementById('dep-time').value,
      driver_name: document.getElementById('driver').value.trim(),
      customer_name: document.getElementById('customer').value.trim(),
      invoices: invItems 
    };

    try {
      await fetch(GOOGLE_SCRIPT_URL, {
        method: 'POST',
        mode: 'no-cors',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(payload)
      });

      setTimeout(() => {
        document.getElementById('driver').value = '';
        document.getElementById('customer').value = '';
        document.getElementById('invoices-container').innerHTML = `
          <div class="invoice-item grid grid-cols-12 gap-2 items-center bg-slate-700/20 p-2 rounded-xl border border-slate-700">
            <div class="col-span-4">
             <select class="inv-prefix w-full bg-slate-700 border border-slate-600 rounded-lg px-2 py-2 text-white text-sm focus:outline-none"> 
              <option value="INVB-">INVB-</option> <option value="INVN-">INVN-</option> <option value="INMB-">INMB-</option> <option value="INMN-">INMN-</option> 
             </select>
            </div>
            <div class="col-span-5">
             <input type="text" required class="inv-number w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-1.5 text-white text-sm focus:outline-none" placeholder="เลขที่เอกสาร">
            </div>
            <div class="col-span-2">
             <input type="text" value="2026" readonly class="inv-year w-full bg-slate-800 border border-slate-700 rounded-lg px-1 py-1.5 text-slate-500 text-sm text-center font-bold">
            </div>
            <div class="col-span-1 text-center">
             <button type="button" class="remove-invoice-btn text-red-400 hover:text-red-600 p-1"><i data-lucide="x-circle" class="w-5 h-5 mx-auto"></i></button>
            </div>
          </div>
        `;
        subBtn.disabled = false;
        subBtn.innerHTML = '<i data-lucide="save" class="w-5 h-5"></i> บันทึกข้อมูลขึ้นชีตแยกแถว';
        fetchRecords(); 
      }, 1200);
    } catch(err) {
      alert('บันทึกล้มเหลว');
      subBtn.disabled = false;
    }
  });
  </script>
 </body>
</html>
