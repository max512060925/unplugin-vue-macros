<script setup lang="ts">
export interface Props {
  color: string
}

const { foo } = defineModel<{
  foo: string
}>()

withDefaults(defineProps<Props>(), {
  color: 'blue'
})

console.log(foo)
</script>
