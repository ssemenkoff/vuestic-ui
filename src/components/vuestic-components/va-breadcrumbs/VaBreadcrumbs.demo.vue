<template>
  <VbDemo>
    <VbCard title="default">
      <va-breadcrumbs>
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
    </VbCard>

    <VbCard title="routes">
      <va-breadcrumbs>
        <va-breadcrumbs-item
          label="One"
          to="#one"
        />
        <va-breadcrumbs-item
          label="Two"
          to="#two"
        />
        <va-breadcrumbs-item
          label="Three"
          to="#three"
        />
      </va-breadcrumbs>
    </VbCard>

    <VbCard
      title="Align"
      width="300px"
    >
      Left:
      <va-breadcrumbs align="left">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
      Center:
      <va-breadcrumbs align="center">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
      Right:
      <va-breadcrumbs align="right">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
      Between:
      <va-breadcrumbs align="between">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
      Around:
      <va-breadcrumbs align="around">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
    </VbCard>

    <VbCard title="Color">
      Color:
      <va-breadcrumbs color="danger">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
      Separator color:
      <va-breadcrumbs separator-color="danger">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
      Active color:
      <va-breadcrumbs active-color="danger">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
    </VbCard>

    <VbCard title="Separator">
      Custom separator:
      <va-breadcrumbs separator=">">
        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
      Slotted separator:
      <va-breadcrumbs>
        <template v-slot:separator>
          👌
        </template>

        <va-breadcrumbs-item label="One" />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
      <br>
    </VbCard>

    <VbCard title="Disabled">
      <va-breadcrumbs>
        <va-breadcrumbs-item
          disabled
          label="One"
        />
        <va-breadcrumbs-item
          disabled
          label="Two"
        />
        <va-breadcrumbs-item
          disabled
          label="Three"
        />
      </va-breadcrumbs>
      <br>
      With routes
      <va-breadcrumbs>
        <va-breadcrumbs-item
          disabled
          label="One"
          to="#one"
        />
        <va-breadcrumbs-item
          label="Two"
          to="#two"
        />
        <va-breadcrumbs-item
          label="Three"
          to="#three"
        />
      </va-breadcrumbs>
      <br>
      Active color + disabled:
      <va-breadcrumbs active-color="primary">
        <va-breadcrumbs-item
          disabled
          label="One"
        />
        <va-breadcrumbs-item label="Two" />
        <va-breadcrumbs-item label="Three" />
      </va-breadcrumbs>
    </VbCard>
  </VbDemo>
</template>

<script>
import VaBreadcrumbs from './VaBreadcrumbs'
import VaBreadcrumbsItem from './VaBreadcrumbsItem'

export default {
  components: {
    VaBreadcrumbs,
    VaBreadcrumbsItem,
  },
}
</script>
