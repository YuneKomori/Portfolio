<script>
    import { Table } from '@skeletonlabs/skeleton';
  
    // ヘッダーとデータ行の正しい形式を定義
    const tableData = {
      head: ['Header 1', 'Header 2', 'Header 3'], // ヘッダーを配列として定義
      body: [
        ['Row 1, Cell 1', 'Row 1, Cell 2', 'Row 1, Cell 3'],  // 各行のセルを配列として定義
        ['Row 2, Cell 1', 'Row 2, Cell 2', 'Row 2, Cell 3']
      ]
    };
  </script>
  
  <Table class="striped" source={tableData} />
  
  