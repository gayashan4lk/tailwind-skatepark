<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf';
  import Card from './card.svelte';

  const { Story } = defineMeta({
    title: 'Card',
    component: Card,
    argTypes: {
      title: {
        control: 'text',
        description: 'Card title',
      },
      description: {
        control: 'text',
        description: 'Card description',
      },
    },
    args: {
      title: 'School of Fish',
      description:
        'A school of fish is a coordinated group of fish, often of the same species, that swim together in a synchronized, unified direction.',
    },
  });
</script>

<Story name="Default" />
