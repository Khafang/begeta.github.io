<template>
  <div class="pd-10px">
    <h1>Justify Self</h1>
    <div>เป็น Atomic Class ที่ใช้เพื่อระบุการจัดวางของตัว Flex Item เอง ใช้ Justify Self เพื่อจัดในแกน Main-Axis</div>

    <h3>Property</h3>
    <table-atomic :data="property"></table-atomic>

    <h3>Value</h3>
    <table-atomic :data="value"></table-atomic>

    <h3>Responsive YES</h3>
    <table-atomic :data="responsive"></table-atomic>

    <h3>Hover NO</h3>
  </div>
</template>

<script>
import TableAtomic from '@/components/TableAtomic'
export default {
  components: {
    TableAtomic
  },
  data () {
    return {
      property: [
        ['Class', 'jtf-s'],
        ['Property', 'justify-self']
      ],
      value: {
        class: [
          'Class',
          'start',
          'end',
          'left',
          'right',
          'flex-start',
          'flex-end',
          'self-start',
          'self-end',
          'strecth'
        ],
        description: [
          'Value Description',
          'สำหรับ "start"',
          'สำหรับ "end"',
          'สำหรับ "left"',
          'สำหรับ "right"',
          'สำหรับ "flex-start"',
          'สำหรับ "flex-end"',
          'สำหรับ "self-start"',
          'สำหรับ "self-end"',
          'สำหรับ "strecth"'
        ]  
      },
      responsive: [
        ['Class', 'mobile', 'tablet', 'desktop', 'widescreen'],
        ['Breakpoints', 'up to 768px', 'from 769px', 'from 1024px', 'from 1408px']
      ]
    }
  }
}
</script>

