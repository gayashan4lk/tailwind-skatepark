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
      title: 'Title of Card',
      description:
        'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which dont look even slightly believable.',
    },
  });
</script>

<Story name="Default" />
