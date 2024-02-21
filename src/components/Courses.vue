<template>
  <v-container>
    <div id="homepage">
      <v-layout column>
        <v-carousel>
          <v-carousel-item
            src="https://strathmore.edu/wp-content/themes/strathmore/images/student-life.webp"
            alt="student life"
          >
            cover ></v-carousel-item
          >

          <v-carousel-item
            src="https://strathmore.edu/wp-content/themes/strathmore/images/slider6.webp"
          >
            cover ></v-carousel-item
          >

          <v-carousel-item
            src="https://strathmore.edu/wp-content/uploads/2023/05/student-life.webp"
          >
            cover ></v-carousel-item
          >
        </v-carousel>
      </v-layout>
      <v-layout>
        <v-container>
          <v-row align="center" justify="center">
            <div class="d-flex align-center flex-column">
              <div class="mt-4 text-subtitle-2">With slots</div>

              <v-card width="600">
                <template v-slot:title>{{ componentTitle }} </template>

                <template v-slot:text>
                  <v-list
                    :items="courses"
                    item-title="coursename"
                    item-value="id"
                  ></v-list>
                </template>
              </v-card>
            </div>
          </v-row>
        </v-container>
      </v-layout></div
  ></v-container>
</template>
<script>
export default {
  // Properties returned from data() become reactive state
  // and will be exposed on `this`.
  data() {
    return {
      courses: [
        {
          id: 1,
          coursename: "Financial Economics",
        },
        {
          id: 2,
          coursename: "Psychology",
        },
        {
          id: 3,
          coursename: "Computer Science",
        },
        {
          id: 4,
          coursename: "Medicine and Surgery",
        },
        {
          id: 5,
          coursename: "Education",
        },
        {
          id: 6,
          coursename: "Architecture",
        },
        {
          id: 7,
          coursename: "Forestry",
        },
        {
          id: 8,
          coursename: "Law",
        },
        {
          id: 9,
          coursename: "Hospitality and Tourism",
        },
        {
          id: 10,
          coursename: "Financial Engineering",
        },
      ],
      componentTitle: "Courses at Strath Uni",
    };
  },

  // Methods are functions that mutate state and trigger updates.
  // They can be bound as event handlers in templates.
  methods: {
    increment() {
      this.count++;
    },
  },

  // Lifecycle hooks are called at different stages
  // of a component's lifecycle.
  // This function will be called when the component is mounted.
  mounted() {
    console.log(`The initial count is ${this.count}.`);
  },
};
</script>
